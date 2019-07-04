---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: ead6c48496c646b5184f88aeac64fbe650be17c4
ms.sourcegitcommit: a4e527d3deba004007cfa22fa536e8255dd23b37
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/02/2019
ms.locfileid: "67516798"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="5e72c-103">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5e72c-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="5e72c-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="5e72c-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="5e72c-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="5e72c-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="5e72c-106">Não existem outros métodos de instalação suportados atualmente para o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="5e72c-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="5e72c-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="5e72c-107">Requirements</span></span>

<span data-ttu-id="5e72c-108">O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell Core 6.x e posterior em todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="5e72c-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="5e72c-109">Se não tiver a certeza se tem o PowerShell, ou está no macOS ou Linux, [instale a versão mais recente do PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span><span class="sxs-lookup"><span data-stu-id="5e72c-109">If you aren't sure if you have PowerShell, or are on macOS or Linux, [install the latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span></span>

<span data-ttu-id="5e72c-110">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="5e72c-110">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="5e72c-111">Para executar o Azure PowerShell no PowerShell 5.1 no Windows:</span><span class="sxs-lookup"><span data-stu-id="5e72c-111">To run Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="5e72c-112">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário.</span><span class="sxs-lookup"><span data-stu-id="5e72c-112">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="5e72c-113">Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="5e72c-113">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="5e72c-114">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="5e72c-114">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

<span data-ttu-id="5e72c-115">Não existem requisitos adicionais para o Azure PowerShell quando utilizar o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="5e72c-115">There are no additional requirements for Azure PowerShell when using PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="5e72c-116">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5e72c-116">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="5e72c-117">__Não__ pode ter os módulos AzureRM e Az instalados em simultâneo para o PowerShell 5.1 para Windows.</span><span class="sxs-lookup"><span data-stu-id="5e72c-117">You __can't__ have both the AzureRM and Az modules installed for PowerShell 5.1 for Windows at the same time.</span></span> <span data-ttu-id="5e72c-118">Se precisar de manter o AzureRM disponível no sistema, instale o módulo do Az para o PowerShell Core 6.x ou posterior.</span><span class="sxs-lookup"><span data-stu-id="5e72c-118">If you need to keep AzureRM available on your system, install the Az module for PowerShell Core 6.x or later.</span></span> <span data-ttu-id="5e72c-119">Para tal, [instale o PowerShell Core 6.x ou posterior](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows) e, em seguida, siga estas instruções num terminal do PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="5e72c-119">To do this, [install PowerShell Core 6.x or later](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows) and then follow these instructions in a PowerShell Core terminal.</span></span>

<span data-ttu-id="5e72c-120">Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e72c-120">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="5e72c-121">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):</span><span class="sxs-lookup"><span data-stu-id="5e72c-121">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="5e72c-122">Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.</span><span class="sxs-lookup"><span data-stu-id="5e72c-122">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="5e72c-123">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="5e72c-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="5e72c-124">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="5e72c-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="5e72c-125">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="5e72c-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="5e72c-126">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e72c-126">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="5e72c-127">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="5e72c-127">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5e72c-128">Resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="5e72c-128">Troubleshooting</span></span>

<span data-ttu-id="5e72c-129">Seguem-se alguns problemas comuns vistos durante a instalação do módulo do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e72c-129">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="5e72c-130">Se detetar um problema não mencionado neste artigo, [registe um problema no GitHub](https://github.com/azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="5e72c-130">If you experience a problem not listed here, please [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="5e72c-131">O proxy bloqueia a ligação</span><span class="sxs-lookup"><span data-stu-id="5e72c-131">Proxy blocks connection</span></span>

<span data-ttu-id="5e72c-132">Se ocorrerem erros de `Install-Module` que indiquem que a Galeria do PowerShell não está acessível, pode estar atrás de um proxy.</span><span class="sxs-lookup"><span data-stu-id="5e72c-132">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="5e72c-133">Diferentes sistemas operativos têm requisitos diferentes para configurar um proxy ao nível do sistema, não abordados detalhadamente aqui.</span><span class="sxs-lookup"><span data-stu-id="5e72c-133">Different operating systems will have different requirements for configuring a system-wide proxy, which are not covered in detail here.</span></span> <span data-ttu-id="5e72c-134">Contacte o administrador de sistema para obter as suas definições de proxy e saber como configurá-las para o seu SO.</span><span class="sxs-lookup"><span data-stu-id="5e72c-134">Contact your system administrator for your proxy settings and how to configure them for your OS.</span></span>

<span data-ttu-id="5e72c-135">O PowerShell não pode ser configurado para utilizar este proxy automaticamente.</span><span class="sxs-lookup"><span data-stu-id="5e72c-135">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="5e72c-136">Com o PowerShell 5.1 e posterior, pode configurar o proxy a utilizar numa sessão do PowerShell com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5e72c-136">With PowerShell 5.1 and later, configure the proxy to use for a PowerShell session with the following command:</span></span>

```powershell
(New-Object System.Net.WebClient).Proxy.Credentials = `
  [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="5e72c-137">Se as credenciais do seu sistema operativo estiverem configuradas corretamente, os pedidos do PowerShell serão encaminhados através do proxy.</span><span class="sxs-lookup"><span data-stu-id="5e72c-137">If your operating system credentials are configured correctly, this will route PowerShell requests through the proxy.</span></span>
<span data-ttu-id="5e72c-138">Para manter esta definição entre sessões, adicione o comando a um [perfil do PowerShell](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="5e72c-138">In order to have this setting persist between sessions, add the command to a [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="5e72c-139">Para instalar o pacote, o proxy tem de permitir ligações HTTPS no seguinte endereço:</span><span class="sxs-lookup"><span data-stu-id="5e72c-139">In order to install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="5e72c-140">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="5e72c-140">Sign in</span></span>

<span data-ttu-id="5e72c-141">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="5e72c-141">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="5e72c-142">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="5e72c-142">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="5e72c-143">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="5e72c-143">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="5e72c-144">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="5e72c-144">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="5e72c-145">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="5e72c-145">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="5e72c-146">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5e72c-146">Update the Azure PowerShell module</span></span>

<span data-ttu-id="5e72c-147">Devido à forma como o módulo do Az é empacotado, o comando [Update-Module](/powershell/module/powershellget/update-module) não atualizará a sua instalação corretamente.</span><span class="sxs-lookup"><span data-stu-id="5e72c-147">Because of how the Az module is packaged, the [Update-Module](/powershell/module/powershellget/update-module) command won't update your installation correctly.</span></span> <span data-ttu-id="5e72c-148">O AZ é tecnicamente um meta-módulo que abrange todos os submódulos que contêm cmdlets para interagir com os serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="5e72c-148">Az is technically a meta-module, encompassing all of the submodules that contain cmdlets to interact with Azure services.</span></span> <span data-ttu-id="5e72c-149">Isso significa que para atualizar o módulo do Azure PowerShell, terá de o __reinstalar__, em vez de apenas o __atualizar__.</span><span class="sxs-lookup"><span data-stu-id="5e72c-149">That means that to update the Azure PowerShell module, you will need to __reinstall__, rather than just __update__.</span></span> <span data-ttu-id="5e72c-150">Isto é feito como a instalação, mas poderá ter de adicionar o argumento `-Force`:</span><span class="sxs-lookup"><span data-stu-id="5e72c-150">This is done in the same way as installing, but you may need to add the `-Force` argument:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="5e72c-151">Embora os módulos instalados possam ser substituídos, poderá ainda ter versões antigas no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="5e72c-151">Although this can overwrite installed modules, you may still have older versions left on your system.</span></span>
<span data-ttu-id="5e72c-152">Para obter mais informações sobre como remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="5e72c-152">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="5e72c-153">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5e72c-153">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="5e72c-154">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e72c-154">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="5e72c-155">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5e72c-155">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="5e72c-156">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="5e72c-156">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="5e72c-157">Pode instalar ou carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="5e72c-157">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="5e72c-158">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="5e72c-158">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="5e72c-159">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="5e72c-159">Provide feedback</span></span>

<span data-ttu-id="5e72c-160">Se encontrar um erro no Azure Powershell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="5e72c-160">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="5e72c-161">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="5e72c-161">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e72c-162">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="5e72c-162">Next Steps</span></span>

<span data-ttu-id="5e72c-163">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="5e72c-163">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="5e72c-164">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="5e72c-164">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>