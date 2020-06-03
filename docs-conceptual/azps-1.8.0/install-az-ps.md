---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/22/2019
ms.openlocfilehash: 88df7d916dd234c51d8982fb63547b5147f9cde8
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84121617"
---
# <a name="install-azure-powershell"></a><span data-ttu-id="90d9c-103">Instalar o Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90d9c-103">Install Azure PowerShell</span></span>

<span data-ttu-id="90d9c-104">Este artigo explica como instalar os módulos do Azure PowerShell com o [PowerShellGet](/powershell/scripting/gallery/installing-psget).</span><span class="sxs-lookup"><span data-stu-id="90d9c-104">This article explains how to install the Azure PowerShell modules using [PowerShellGet](/powershell/scripting/gallery/installing-psget).</span></span> <span data-ttu-id="90d9c-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="90d9c-105">These instructions work on Windows, macOS, and Linux platforms.</span></span>

<span data-ttu-id="90d9c-106">O Azure PowerShell também está disponível no Azure [Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="90d9c-106">Azure PowerShell is also available in Azure [Cloud Shell](/azure/cloud-shell/overview).</span></span>

## <a name="requirements"></a><span data-ttu-id="90d9c-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="90d9c-107">Requirements</span></span>

> [!NOTE]
> <span data-ttu-id="90d9c-108">A versão recomendada do PowerShell para utilização com o Azure PowerShell em todas as plataformas é o PowerShell 7.x e posteriores.</span><span class="sxs-lookup"><span data-stu-id="90d9c-108">PowerShell 7.x and later is the recommended version of PowerShell for use with Azure PowerShell on all platforms.</span></span>

<span data-ttu-id="90d9c-109">O Azure PowerShell funciona com o PowerShell 6.2.4 e posteriores em todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="90d9c-109">Azure PowerShell works with PowerShell 6.2.4 and later on all platforms.</span></span> <span data-ttu-id="90d9c-110">Também é suportado com o PowerShell 5.1 no Windows.</span><span class="sxs-lookup"><span data-stu-id="90d9c-110">It is also supported with PowerShell 5.1 on Windows.</span></span> <span data-ttu-id="90d9c-111">Instale a [versão mais recente do PowerShell](/powershell/scripting/install/installing-powershell) disponível para o seu sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="90d9c-111">Install the [latest version of PowerShell](/powershell/scripting/install/installing-powershell) available for your operating system.</span></span> <span data-ttu-id="90d9c-112">O Azure PowerShell não tem requisitos adicionais quando é executado no PowerShell 6.2.4 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="90d9c-112">Azure PowerShell has no additional requirements when run on PowerShell 6.2.4 and later.</span></span>

<span data-ttu-id="90d9c-113">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="90d9c-113">To check your PowerShell version, run the command:</span></span>

```azurepowershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="90d9c-114">Para utilizar o Azure PowerShell no PowerShell 5.1 no Windows:</span><span class="sxs-lookup"><span data-stu-id="90d9c-114">To use Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="90d9c-115">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="90d9c-115">Update to [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell).</span></span>
   <span data-ttu-id="90d9c-116">Se utilizar o Windows 10, versão 1607 ou superior, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="90d9c-116">If you're on Windows 10 version 1607 or higher, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="90d9c-117">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="90d9c-117">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>
3. <span data-ttu-id="90d9c-118">Verifique se tem a versão mais recente do PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="90d9c-118">Make sure you have the latest version of PowerShellGet.</span></span> <span data-ttu-id="90d9c-119">Execute `Install-Module -Name PowerShellGet -Force`.</span><span class="sxs-lookup"><span data-stu-id="90d9c-119">Run `Install-Module -Name PowerShellGet -Force`.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="90d9c-120">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90d9c-120">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="90d9c-121">Não suportamos os módulos do AzureRM e do Az instalados em simultâneo para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="90d9c-121">We do not support having both the AzureRM and Az modules installed for PowerShell 5.1 on Windows at the same time.</span></span> <span data-ttu-id="90d9c-122">Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell Core 6.x ou posterior.</span><span class="sxs-lookup"><span data-stu-id="90d9c-122">If you need to keep AzureRM available on your system, install the Az module for PowerShell Core 6.x or later.</span></span>

<span data-ttu-id="90d9c-123">A utilização dos cmdlets do PowerShellGet é o método de instalação preferido.</span><span class="sxs-lookup"><span data-stu-id="90d9c-123">Using the PowerShellGet cmdlets is the preferred installation method.</span></span> <span data-ttu-id="90d9c-124">Instale o módulo do Az apenas no utilizador atual.</span><span class="sxs-lookup"><span data-stu-id="90d9c-124">Install the Az module for the current user only.</span></span> <span data-ttu-id="90d9c-125">Este é o âmbito de instalação recomendado.</span><span class="sxs-lookup"><span data-stu-id="90d9c-125">This is the recommended installation scope.</span></span> <span data-ttu-id="90d9c-126">Este método funciona da mesma forma nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="90d9c-126">This method works the same on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="90d9c-127">Execute o seguinte comando a partir de uma sessão do PowerShell:</span><span class="sxs-lookup"><span data-stu-id="90d9c-127">Run the following command from a PowerShell session:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope CurrentUser
}
```

<span data-ttu-id="90d9c-128">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="90d9c-128">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="90d9c-129">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="90d9c-129">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="90d9c-130">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="90d9c-130">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="90d9c-131">A instalação do módulo para todos os utilizadores num sistema requer privilégios elevados.</span><span class="sxs-lookup"><span data-stu-id="90d9c-131">Installing the module for all users on a system requires elevated privileges.</span></span> <span data-ttu-id="90d9c-132">Inicie a sessão do PowerShell com a opção **Executar como administrador** no Windows ou utilize o comando `sudo` no macOS ou Linux:</span><span class="sxs-lookup"><span data-stu-id="90d9c-132">Start the PowerShell session using **Run as administrator** in Windows or use the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Scope AllUsers
}
```

<span data-ttu-id="90d9c-133">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d9c-133">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="90d9c-134">A instalação do mesmo transfere todos os módulos do Az do PowerShell em disponibilidade geral e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="90d9c-134">Installing it downloads all of the generally available Az PowerShell modules, and makes their cmdlets available for use.</span></span>

## <a name="install-offline"></a><span data-ttu-id="90d9c-135">Instalar offline</span><span class="sxs-lookup"><span data-stu-id="90d9c-135">Install offline</span></span>

<span data-ttu-id="90d9c-136">Em alguns ambientes, não é possível ligar à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d9c-136">In some environments, it's not possible to connect to the PowerShell Gallery.</span></span> <span data-ttu-id="90d9c-137">Nessas situações, ainda pode instalar offline através de um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="90d9c-137">In those situations, you can still install offline using one of these methods:</span></span>

* <span data-ttu-id="90d9c-138">Transfira os módulos para outra localização na sua rede e utilize-os como uma origem de instalação.</span><span class="sxs-lookup"><span data-stu-id="90d9c-138">Download the modules to another location in your network and use that as an installation source.</span></span>
  <span data-ttu-id="90d9c-139">Este método permite-lhe colocar em cache os módulos do PowerShell num único servidor ou que seja implementada a partilha de ficheiros através do PowerShellGet para quaisquer sistemas desligados.</span><span class="sxs-lookup"><span data-stu-id="90d9c-139">This method allows you to cache PowerShell modules on a single server or file share to be deployed with PowerShellGet to any disconnected systems.</span></span> <span data-ttu-id="90d9c-140">Saiba como configurar um repositório local e instalar em sistemas desligados com a opção [Trabalhar com repositórios do PowerShellGet locais](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span><span class="sxs-lookup"><span data-stu-id="90d9c-140">Learn how to set up a local repository and install on disconnected systems with [Working with local PowerShellGet repositories](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span></span>
* <span data-ttu-id="90d9c-141">[Transferira o MSI do Azure PowerShell](install-az-ps-msi.md) para um computador ligado a uma rede e, em seguida, copie o instalador para os sistemas sem o acesso à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d9c-141">[Download the Azure PowerShell MSI](install-az-ps-msi.md) to a machine connected to the network, and then copy the installer to systems without access to PowerShell Gallery.</span></span> <span data-ttu-id="90d9c-142">Tenha em mente que o instalador MSI funciona apenas para o PowerShell 5.1 no Windows.</span><span class="sxs-lookup"><span data-stu-id="90d9c-142">Keep in mind that the MSI installer only works for PowerShell 5.1 on Windows.</span></span>
* <span data-ttu-id="90d9c-143">Guarde o módulo com [Guardar-Módulo](/powershell/module/PowershellGet/Save-Module) numa partilha de ficheiros ou guarde noutra fonte e faça a cópia manualmente para outros computadores:</span><span class="sxs-lookup"><span data-stu-id="90d9c-143">Save the module with [Save-Module](/powershell/module/PowershellGet/Save-Module) to a file share, or save it to another source and manually copy it to other machines:</span></span>

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a><span data-ttu-id="90d9c-144">Resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="90d9c-144">Troubleshooting</span></span>

<span data-ttu-id="90d9c-145">Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d9c-145">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="90d9c-146">Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="90d9c-146">If you experience a problem not listed here, [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="90d9c-147">O proxy bloqueia a ligação</span><span class="sxs-lookup"><span data-stu-id="90d9c-147">Proxy blocks connection</span></span>

<span data-ttu-id="90d9c-148">Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy.</span><span class="sxs-lookup"><span data-stu-id="90d9c-148">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="90d9c-149">Diferentes sistemas operativos e ambientes de rede têm requisitos diferentes para configurar um proxy ao nível do sistema.</span><span class="sxs-lookup"><span data-stu-id="90d9c-149">Different operating systems and network environment have different requirements for configuring a system-wide proxy.</span></span> <span data-ttu-id="90d9c-150">Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="90d9c-150">Contact your system administrator for your proxy settings and how to configure them for your environment.</span></span>

<span data-ttu-id="90d9c-151">O PowerShell não pode ser configurado para utilizar este proxy automaticamente.</span><span class="sxs-lookup"><span data-stu-id="90d9c-151">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="90d9c-152">Com o PowerShell 5.1 e posterior, pode configurar a sessão do PowerShell para utilizar um proxy com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="90d9c-152">With PowerShell 5.1 and later, configure the PowerShell session to use a proxy using the following commands:</span></span>

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="90d9c-153">Se as credenciais do seu sistema operativo estiverem configuradas corretamente, esta configuração encaminha os pedidos do PowerShell através do proxy.</span><span class="sxs-lookup"><span data-stu-id="90d9c-153">If your operating system credentials are configured correctly, this configuration routes PowerShell requests through the proxy.</span></span> <span data-ttu-id="90d9c-154">Para manter esta definição entre sessões, adicione os comandos ao seu [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="90d9c-154">To have this setting persist between sessions, add the commands to your [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="90d9c-155">Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="90d9c-155">To install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="90d9c-156">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="90d9c-156">Sign in</span></span>

<span data-ttu-id="90d9c-157">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="90d9c-157">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="90d9c-158">Se tiver desativado o carregamento automático do módulo, importe o módulo manualmente com `Import-Module -Name Az`.</span><span class="sxs-lookup"><span data-stu-id="90d9c-158">If you've disabled module autoloading, manually import the module with `Import-Module -Name Az`.</span></span>
> <span data-ttu-id="90d9c-159">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="90d9c-159">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="90d9c-160">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="90d9c-160">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="90d9c-161">Para saber como manter o início de sessão do Azure entre sessões do PowerShell, veja [Manter as credenciais do utilizador entre sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-161">To learn how to persist your Azure sign in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="90d9c-162">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90d9c-162">Update the Azure PowerShell module</span></span>

<span data-ttu-id="90d9c-163">Para atualizar qualquer módulo do PowerShell, deve utilizar o mesmo método utilizado para instalar o módulo.</span><span class="sxs-lookup"><span data-stu-id="90d9c-163">To update any PowerShell module, you should use the same method used to install the module.</span></span> <span data-ttu-id="90d9c-164">Por exemplo, se utilizou originalmente `Install-Module`, deve utilizar [Update-Module](/powershell/module/powershellget/update-module) para obter a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="90d9c-164">For example, if you originally used `Install-Module`, then you should use [Update-Module](/powershell/module/powershellget/update-module) to get the latest version.</span></span> <span data-ttu-id="90d9c-165">Se utilizou originalmente o pacote MSI, deve transferir e instalar o novo pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="90d9c-165">If you originally used the MSI package then you should download and install the new MSI package.</span></span>

<span data-ttu-id="90d9c-166">Os cmdlets do PowerShellGet não conseguem atualizar os módulos instalados a partir de um pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="90d9c-166">The PowerShellGet cmdlets cannot update modules that were installed from an MSI package.</span></span> <span data-ttu-id="90d9c-167">Os pacotes MSI não atualizam os módulos instalados com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="90d9c-167">MSI packages do not update modules that were installed using PowerShellGet.</span></span> <span data-ttu-id="90d9c-168">Se tiver problemas ao utilizar o PowershellGet, deve **reinstalá-lo**, em vez de **o atualizar**.</span><span class="sxs-lookup"><span data-stu-id="90d9c-168">If you have any issues updating using PowershellGet, then you should **reinstall**, rather than **update**.</span></span> <span data-ttu-id="90d9c-169">A reinstalação é feita como a instalação, mas terá ter de adicionar o parâmetro `-Force`:</span><span class="sxs-lookup"><span data-stu-id="90d9c-169">Reinstalling is done the same way as installing, but you need to add the `-Force` parameter:</span></span>

```powershell
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
      'Az modules installed at the same time is not supported.')
} else {
    Install-Module -Name Az -AllowClobber -Force
}
```

<span data-ttu-id="90d9c-170">Ao contrário das instalações baseadas em MSI, instalar ou atualizar com o PowerShellGet não remove as versões mais antigas que possam existir no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="90d9c-170">Unlike MSI-based installations, installing or updating using PowerShellGet does not remove older versions that may exist on your system.</span></span> <span data-ttu-id="90d9c-171">Para remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-171">To remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span> <span data-ttu-id="90d9c-172">Para obter mais informações sobre instalações baseadas em MSI, veja [Instalar o Azure PowerShell com um MSI](install-az-ps-msi.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-172">For more information about MSI-based installations, see [Install Azure PowerShell with an MSI](install-az-ps-msi.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="90d9c-173">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="90d9c-173">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="90d9c-174">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90d9c-174">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="90d9c-175">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="90d9c-175">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | Select-Object -Property Name, Version
```

<span data-ttu-id="90d9c-176">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-176">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="90d9c-177">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="90d9c-177">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

<span data-ttu-id="90d9c-178">Pode instalar ou carregar uma versão específica do módulo `Az` com o parâmetro `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="90d9c-178">You can install or load a specific version of the `Az` module using the `-RequiredVersion` parameter:</span></span>

```powershell-interactive
# Install Az version 1.8.0
Install-Module -Name Az -RequiredVersion 1.8.0
# Load Az version 1.8.0
Import-Module -Name Az -RequiredVersion 1.8.0
```

## <a name="provide-feedback"></a><span data-ttu-id="90d9c-179">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="90d9c-179">Provide feedback</span></span>

<span data-ttu-id="90d9c-180">Se encontrar um erro no Azure PowerShell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="90d9c-180">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="90d9c-181">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="90d9c-181">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="90d9c-182">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="90d9c-182">Next Steps</span></span>

<span data-ttu-id="90d9c-183">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-183">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="90d9c-184">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="90d9c-184">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
