---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: d99265c7f156622d876d700106e2b06dd729e8b8
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365753"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="374a4-103">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="374a4-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="374a4-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="374a4-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="374a4-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="374a4-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="374a4-106">Não existem outros métodos de instalação suportados atualmente para o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="374a4-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="374a4-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="374a4-107">Requirements</span></span>

<span data-ttu-id="374a4-108">O Azure PowerShell funciona com o PowerShell 5.1 ou superior no Windows, ou com o PowerShell Core 6.x e posterior em todas as plataformas.</span><span class="sxs-lookup"><span data-stu-id="374a4-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="374a4-109">Se não tiver a certeza se tem o PowerShell, ou está no macOS ou Linux, [instale a versão mais recente do PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span><span class="sxs-lookup"><span data-stu-id="374a4-109">If you aren't sure if you have PowerShell, or are on macOS or Linux, [install the latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span></span>

<span data-ttu-id="374a4-110">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="374a4-110">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="374a4-111">Para executar o Azure PowerShell no PowerShell 5.1 no Windows:</span><span class="sxs-lookup"><span data-stu-id="374a4-111">To run Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="374a4-112">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário.</span><span class="sxs-lookup"><span data-stu-id="374a4-112">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="374a4-113">Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="374a4-113">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="374a4-114">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="374a4-114">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

<span data-ttu-id="374a4-115">Não existem requisitos adicionais para o Azure PowerShell quando utilizar o PowerShell Core.</span><span class="sxs-lookup"><span data-stu-id="374a4-115">There are no additional requirements for Azure PowerShell when using PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="374a4-116">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="374a4-116">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="374a4-117">Pode ter ambos os módulos, AzureRM e Az, instalados em simultâneo.</span><span class="sxs-lookup"><span data-stu-id="374a4-117">You can have both the AzureRM and Az modules installed at the same time.</span></span> <span data-ttu-id="374a4-118">Se tiver ambos os módulos instalados, __não ative os aliases__.</span><span class="sxs-lookup"><span data-stu-id="374a4-118">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="374a4-119">A ativação dos aliases irá causar conflitos entre os cmdlets do AzureRM e os aliases de comandos do Az, o que pode dar origem a um comportamento inesperado.</span><span class="sxs-lookup"><span data-stu-id="374a4-119">Enabling aliases will cause conflicts between AzureRM cmdlets and Az command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="374a4-120">Recomenda-se que desinstale o AzureRM antes de instalar o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="374a4-120">It's recommended that before installing the Az module, you uninstall AzureRM.</span></span> <span data-ttu-id="374a4-121">Pode sempre desinstalar o AzureRM ou ativar os aliases em qualquer altura.</span><span class="sxs-lookup"><span data-stu-id="374a4-121">You can always uninstall AzureRM or enable aliases at any time.</span></span> <span data-ttu-id="374a4-122">Para obter mais informações sobre os aliases de comandos do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-122">To learn about the AzureRM command aliases, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
> <span data-ttu-id="374a4-123">Para obter instruções de desinstalação, veja [Desinstalar o módulo do AzureRM](uninstall-az-ps.md#uninstall-the-azurerm-module).</span><span class="sxs-lookup"><span data-stu-id="374a4-123">For uninstall instructions, see [Uninstall the AzureRM module](uninstall-az-ps.md#uninstall-the-azurerm-module).</span></span> 

<span data-ttu-id="374a4-124">Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="374a4-124">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="374a4-125">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):</span><span class="sxs-lookup"><span data-stu-id="374a4-125">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="374a4-126">Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.</span><span class="sxs-lookup"><span data-stu-id="374a4-126">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="374a4-127">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="374a4-127">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="374a4-128">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="374a4-128">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="374a4-129">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="374a4-129">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="374a4-130">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="374a4-130">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="374a4-131">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="374a4-131">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="374a4-132">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="374a4-132">Sign in</span></span>

<span data-ttu-id="374a4-133">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="374a4-133">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="374a4-134">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="374a4-134">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="374a4-135">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="374a4-135">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="374a4-136">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="374a4-136">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="374a4-137">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-137">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="374a4-138">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="374a4-138">Update the Azure PowerShell module</span></span>

<span data-ttu-id="374a4-139">Devido à forma como o módulo do Az é empacotado, o comando [Update-Module](/powershell/module/powershellget/update-module) não atualizará a sua instalação corretamente.</span><span class="sxs-lookup"><span data-stu-id="374a4-139">Because of how the Az module is package, the [Update-Module](/powershell/module/powershellget/update-module) command won't update your installation correctly.</span></span> <span data-ttu-id="374a4-140">O AZ é tecnicamente um meta-módulo que abrange todos os submódulos que contêm cmdlets para interagir com os serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="374a4-140">Az is technically a meta-module, encompassing all of the submodules that contain cmdlets to interact with Azure services.</span></span> <span data-ttu-id="374a4-141">Isso significa que para atualizar o módulo do Azure PowerShell, terá de o __reinstalar__, em vez de apenas o __atualizar__.</span><span class="sxs-lookup"><span data-stu-id="374a4-141">That means that to update the Azure PowerShell module, you will need to __reinstall__, rather than just __update__.</span></span> <span data-ttu-id="374a4-142">Isto é feito como a instalação, mas poderá ter de adicionar o argumento `-Force`:</span><span class="sxs-lookup"><span data-stu-id="374a4-142">This is done in the same way as installing, but you may need to add the `-Force` argument:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="374a4-143">Embora os módulos instalados possam ser substituídos, poderá ainda ter versões antigas no seu sistema.</span><span class="sxs-lookup"><span data-stu-id="374a4-143">Although this can overwrite installed modules, you may still have older versions left on your system.</span></span>
<span data-ttu-id="374a4-144">Para obter mais informações sobre como remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-144">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="374a4-145">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="374a4-145">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="374a4-146">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="374a4-146">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="374a4-147">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="374a4-147">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="374a4-148">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-148">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="374a4-149">Pode instalar ou carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="374a4-149">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="374a4-150">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="374a4-150">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="374a4-151">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="374a4-151">Provide feedback</span></span>

<span data-ttu-id="374a4-152">Se encontrar um erro no Azure Powershell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="374a4-152">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="374a4-153">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="374a4-153">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="374a4-154">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="374a4-154">Next Steps</span></span>

<span data-ttu-id="374a4-155">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-155">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="374a4-156">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="374a4-156">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
