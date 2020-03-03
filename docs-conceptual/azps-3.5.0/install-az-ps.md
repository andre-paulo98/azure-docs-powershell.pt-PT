---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/22/2019
ms.openlocfilehash: 66d755384e532d434811f3e6122dcba97d5c48b5
ms.sourcegitcommit: a321ef9d134c684fa24ababcbd898f86b00d9364
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "77477853"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="3efa8-103">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3efa8-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="3efa8-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="3efa8-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="3efa8-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="3efa8-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="3efa8-106">Não existem outros métodos de instalação suportados atualmente para o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="3efa8-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="3efa8-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="3efa8-107">Requirements</span></span>

<span data-ttu-id="3efa8-108">O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell Core 6.x e posterior em todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="3efa8-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="3efa8-109">Se não tiver a certeza se tem o PowerShell, ou está no macOS ou Linux, [instale a versão mais recente do PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span><span class="sxs-lookup"><span data-stu-id="3efa8-109">If you aren't sure if you have PowerShell, or are on macOS or Linux, [install the latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span></span>

<span data-ttu-id="3efa8-110">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="3efa8-110">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="3efa8-111">Para executar o Azure PowerShell no PowerShell 5.1 no Windows:</span><span class="sxs-lookup"><span data-stu-id="3efa8-111">To run Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="3efa8-112">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário.</span><span class="sxs-lookup"><span data-stu-id="3efa8-112">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="3efa8-113">Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="3efa8-113">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="3efa8-114">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="3efa8-114">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

<span data-ttu-id="3efa8-115">Não existem requisitos adicionais para o Azure PowerShell quando utilizar o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="3efa8-115">There are no additional requirements for Azure PowerShell when using PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="3efa8-116">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3efa8-116">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="3efa8-117">__Não__ pode ter os módulos AzureRM e Az instalados em simultâneo para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="3efa8-117">You __can't__ have both the AzureRM and Az modules installed for PowerShell 5.1 for Windows at the same time.</span></span> <span data-ttu-id="3efa8-118">Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell Core 6.x ou posterior.</span><span class="sxs-lookup"><span data-stu-id="3efa8-118">If you need to keep AzureRM available on your system, install the Az module for PowerShell Core 6.x or later.</span></span> <span data-ttu-id="3efa8-119">Para tal, [instale o PowerShell Core 6.x ou posterior](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows) e, em seguida, siga estas instruções num terminal do PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="3efa8-119">To do this, [install PowerShell Core 6.x or later](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows) and then follow these instructions in a PowerShell Core terminal.</span></span>

<span data-ttu-id="3efa8-120">O método de instalação recomendado é instalar apenas para o utilizador ativo:</span><span class="sxs-lookup"><span data-stu-id="3efa8-120">The recommended install method is to only install for the active user:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="3efa8-121">Se quiser instalar para todos os utilizadores num sistema, precisará de privilégios de administrador.</span><span class="sxs-lookup"><span data-stu-id="3efa8-121">If you want to install for all users on a system, this requires administrator privileges.</span></span> <span data-ttu-id="3efa8-122">Numa sessão do PowerShell elevada, execute como administrador ou com o comando `sudo` no macOS ou Linux:</span><span class="sxs-lookup"><span data-stu-id="3efa8-122">From an elevated PowerShell session either run as administrator or with the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
```

<span data-ttu-id="3efa8-123">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="3efa8-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="3efa8-124">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="3efa8-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="3efa8-125">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="3efa8-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="3efa8-126">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3efa8-126">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="3efa8-127">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="3efa8-127">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="install-offline"></a><span data-ttu-id="3efa8-128">Instalar offline</span><span class="sxs-lookup"><span data-stu-id="3efa8-128">Install offline</span></span>

<span data-ttu-id="3efa8-129">Em alguns ambientes, não é possível ligar à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3efa8-129">In some environments it's not possible to connect to the PowerShell Gallery.</span></span> <span data-ttu-id="3efa8-130">Nessas situações, ainda pode instalar offline através de um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="3efa8-130">In those situations, you can still install offline using one of these methods:</span></span>

* <span data-ttu-id="3efa8-131">Transfira os módulos para outra localização e utilize-os como uma origem de instalação na sua rede.</span><span class="sxs-lookup"><span data-stu-id="3efa8-131">Download the modules to another location and use that as an installation source on your network.</span></span> <span data-ttu-id="3efa8-132">Isso pode ser um processo complicado, mas irá permitir que armazene em cache os módulos do PowerShell num único servidor ou que seja implementada a partilha de ficheiros através do PowerShellGet para quaisquer sistemas desligados.</span><span class="sxs-lookup"><span data-stu-id="3efa8-132">This can be a complicated process, but will let you cache PowerShell modules on a single server or file share to be deployed with PowerShellGet to any disconnected systems.</span></span> <span data-ttu-id="3efa8-133">Saiba como configurar um repositório local e instalar em sistemas desligados com a opção [Trabalhar com repositórios do PowerShellGet locais](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span><span class="sxs-lookup"><span data-stu-id="3efa8-133">Learn how to set up a local repository and install on disconnected systems with [Working with local PowerShellGet repositories](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span></span>
* <span data-ttu-id="3efa8-134">[Transferira o MSI do Azure PowerShell](install-az-ps-msi.md) para um computador ligado a uma rede e, em seguida, copie o instalador para os sistemas sem o acesso à Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3efa8-134">[Download the Azure PowerShell MSI](install-az-ps-msi.md) to a machine connected to the network, and then copy the installer to systems without access to PowerShell Gallery.</span></span> <span data-ttu-id="3efa8-135">Tenha em mente que o instalador MSI funciona apenas para o PowerShell 5.1 no Windows.</span><span class="sxs-lookup"><span data-stu-id="3efa8-135">Keep in mind that the MSI installer only works for PowerShell 5.1 on Windows.</span></span>
* <span data-ttu-id="3efa8-136">Guarde o módulo com [Guardar-Módulo](/powershell/module/PowershellGet/Save-Module) numa partilha de ficheiros ou guarde noutra fonte e faça a cópia manualmente para outros computadores:</span><span class="sxs-lookup"><span data-stu-id="3efa8-136">Save the module with [Save-Module](/powershell/module/PowershellGet/Save-Module) to a file share, or save it to another source and manually copy it to other machines:</span></span>
  
  ```powershell-interactive
  Save-Module -Name Az -Path '\\someshare\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a><span data-ttu-id="3efa8-137">Resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="3efa8-137">Troubleshooting</span></span>

<span data-ttu-id="3efa8-138">Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3efa8-138">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="3efa8-139">Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="3efa8-139">If you experience a problem not listed here, please [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="3efa8-140">O proxy bloqueia a ligação</span><span class="sxs-lookup"><span data-stu-id="3efa8-140">Proxy blocks connection</span></span>

<span data-ttu-id="3efa8-141">Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy.</span><span class="sxs-lookup"><span data-stu-id="3efa8-141">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="3efa8-142">Diferentes sistemas operativos têm requisitos diferentes para configurar um proxy ao nível do sistema, não abordados detalhadamente aqui.</span><span class="sxs-lookup"><span data-stu-id="3efa8-142">Different operating systems will have different requirements for configuring a system-wide proxy, which are not covered in detail here.</span></span> <span data-ttu-id="3efa8-143">Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu SO.</span><span class="sxs-lookup"><span data-stu-id="3efa8-143">Contact your system administrator for your proxy settings and how to configure them for your OS.</span></span>

<span data-ttu-id="3efa8-144">O PowerShell não pode ser configurado para utilizar este proxy automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3efa8-144">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="3efa8-145">Com o PowerShell 5.1 e posterior, pode configurar o proxy a utilizar numa sessão do PowerShell com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="3efa8-145">With PowerShell 5.1 and later, configure the proxy to use for a PowerShell session with the following command:</span></span>

```powershell
(New-Object System.Net.WebClient).Proxy.Credentials = `
  [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="3efa8-146">Se as credenciais do seu sistema operativo estiverem configuradas corretamente, os pedidos do PowerShell serão encaminhados através do proxy.</span><span class="sxs-lookup"><span data-stu-id="3efa8-146">If your operating system credentials are configured correctly, this will route PowerShell requests through the proxy.</span></span>
<span data-ttu-id="3efa8-147">Para manter esta definição entre sessões, adicione o comando a um [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="3efa8-147">In order to have this setting persist between sessions, add the command to a [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="3efa8-148">Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="3efa8-148">In order to install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="3efa8-149">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="3efa8-149">Sign in</span></span>

<span data-ttu-id="3efa8-150">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="3efa8-150">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="3efa8-151">Se tiver desativado o carregamento automático do módulo, importe o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="3efa8-151">If you've disabled module autoloading, manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="3efa8-152">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="3efa8-152">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="3efa8-153">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="3efa8-153">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="3efa8-154">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="3efa8-154">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="3efa8-155">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3efa8-155">Update the Azure PowerShell module</span></span>

<span data-ttu-id="3efa8-156">Se utilizou originalmente Install-Module, deverá utilizar [Update-Module](/powershell/module/powershellget/update-module) para obter a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="3efa8-156">If you originally used Install-Module, then you should use [Update-Module](/powershell/module/powershellget/update-module) to get the latest version.</span></span> <span data-ttu-id="3efa8-157">Se utilizou originalmente o pacote MSI, deve transferir e instalar o novo MSI para atualizar.</span><span class="sxs-lookup"><span data-stu-id="3efa8-157">If you originally used the MSI package then you should download and install the new MSI in order to udpate.</span></span> <span data-ttu-id="3efa8-158">Se tiver problemas com a atualização com o pacote do PowershellGet, terá de __reinstalar__, em vez de apenas __atualizar__.</span><span class="sxs-lookup"><span data-stu-id="3efa8-158">If you have any issues with updating using the package from PowershellGet then you will need to __reinstall__, rather than just __update__.</span></span> <span data-ttu-id="3efa8-159">Isto é feito como a instalação, mas poderá ter de adicionar o argumento `-Force`:</span><span class="sxs-lookup"><span data-stu-id="3efa8-159">This is done in the same way as installing, but you may need to add the `-Force` argument:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="3efa8-160">Embora os módulos instalados possam ser substituídos, poderá ainda ter versões antigas no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="3efa8-160">Although this can overwrite installed modules, you may still have older versions left on your system.</span></span>
<span data-ttu-id="3efa8-161">Para obter mais informações sobre como remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="3efa8-161">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="3efa8-162">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3efa8-162">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="3efa8-163">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3efa8-163">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="3efa8-164">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="3efa8-164">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="3efa8-165">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="3efa8-165">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="3efa8-166">Pode instalar ou carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="3efa8-166">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="3efa8-167">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="3efa8-167">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="3efa8-168">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="3efa8-168">Provide feedback</span></span>

<span data-ttu-id="3efa8-169">Se encontrar um erro no Azure Powershell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="3efa8-169">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="3efa8-170">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="3efa8-170">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3efa8-171">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="3efa8-171">Next Steps</span></span>

<span data-ttu-id="3efa8-172">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="3efa8-172">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="3efa8-173">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="3efa8-173">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>