---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 828fa8cb2aabac893c566fb146d00af04b16b479
ms.sourcegitcommit: 6685809f054203bd733c84f68acc69e53e5cca8c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982931"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="6170c-103">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6170c-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="6170c-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="6170c-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="6170c-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="6170c-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="6170c-106">Não existem outros métodos de instalação suportados atualmente para o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="6170c-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="6170c-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="6170c-107">Requirements</span></span>

<span data-ttu-id="6170c-108">O Azure PowerShell funciona com o PowerShell 5.x no Windows 7 ou superior, ou com o PowerShell 6.x em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="6170c-108">Azure PowerShell works with PowerShell 5.x on Windows 7 or higher, or PowerShell 6.x on any platform.</span></span>
<span data-ttu-id="6170c-109">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="6170c-109">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="6170c-110">Se tiver uma versão desatualizada ou precisar de instalar o PowerShell, veja [Instalar várias versões do PowerShell](/powershell/scripting/setup/installing-powershell).</span><span class="sxs-lookup"><span data-stu-id="6170c-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](/powershell/scripting/setup/installing-powershell).</span></span> <span data-ttu-id="6170c-111">As informações sobre a instalação da sua plataforma estão associadas a essa página.</span><span class="sxs-lookup"><span data-stu-id="6170c-111">Install information for your platform is linked from that page.</span></span>

<span data-ttu-id="6170c-112">Se estiver a utilizar o PowerShell 5.x no Windows, também precisa de ter o .NET Framework 4.7.2 instalado.</span><span class="sxs-lookup"><span data-stu-id="6170c-112">If you are using PowerShell 5.x on Windows, you also need .NET Framework 4.7.2 installed.</span></span> <span data-ttu-id="6170c-113">Para obter instruções sobre como atualizar ou instalar uma nova versão do .NET Framework, veja o [Guia de instalação do .NET Framework](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="6170c-113">For instructions on updating or installing a new version of .NET Framework, see the [.NET Framework installation guide](/dotnet/framework/install).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="6170c-114">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6170c-114">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="6170c-115">Pode ter ambos os módulos, AzureRM e Az, instalados em simultâneo.</span><span class="sxs-lookup"><span data-stu-id="6170c-115">You can have both the AzureRM and Az modules installed at the same time.</span></span> <span data-ttu-id="6170c-116">Se tiver ambos os módulos instalados, __não ative os aliases__.</span><span class="sxs-lookup"><span data-stu-id="6170c-116">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="6170c-117">A ativação dos aliases irá causar conflitos entre os cmdlets do AzureRM e os aliases de comandos do Az, o que pode dar origem a um comportamento inesperado.</span><span class="sxs-lookup"><span data-stu-id="6170c-117">Enabling aliases will cause conflicts between AzureRM cmdlets and Az command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="6170c-118">Recomenda-se que desinstale o AzureRM antes de instalar o módulo do Az.</span><span class="sxs-lookup"><span data-stu-id="6170c-118">It's recommended that before installing the Az module, you uninstall AzureRM.</span></span> <span data-ttu-id="6170c-119">Pode sempre desinstalar o AzureRM ou ativar os aliases em qualquer altura.</span><span class="sxs-lookup"><span data-stu-id="6170c-119">You can always uninstall AzureRM or enable aliases at any time.</span></span> <span data-ttu-id="6170c-120">Para obter mais informações sobre os aliases de comandos do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-120">To learn about the AzureRM command aliases, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
> <span data-ttu-id="6170c-121">Para obter instruções de desinstalação, veja [Desinstalar o módulo do AzureRM](uninstall-az-ps.md#uninstall-the-azurerm-module).</span><span class="sxs-lookup"><span data-stu-id="6170c-121">For uninstall instructions, see [Uninstall the AzureRM module](uninstall-az-ps.md#uninstall-the-azurerm-module).</span></span> 

<span data-ttu-id="6170c-122">Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6170c-122">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="6170c-123">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):</span><span class="sxs-lookup"><span data-stu-id="6170c-123">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="6170c-124">Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.</span><span class="sxs-lookup"><span data-stu-id="6170c-124">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="6170c-125">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="6170c-125">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="6170c-126">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="6170c-126">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="6170c-127">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="6170c-127">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="6170c-128">O módulo do Az é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6170c-128">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="6170c-129">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="6170c-129">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="6170c-130">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="6170c-130">Sign in</span></span>

<span data-ttu-id="6170c-131">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6170c-131">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="6170c-132">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="6170c-132">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="6170c-133">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="6170c-133">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="6170c-134">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="6170c-134">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="6170c-135">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-135">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="6170c-136">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6170c-136">Update the Azure PowerShell module</span></span>

<span data-ttu-id="6170c-137">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="6170c-137">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="6170c-138">Este comando __não__ desinstala versões mais antigas.</span><span class="sxs-lookup"><span data-stu-id="6170c-138">This command does __not__ uninstall older versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="6170c-139">Para obter mais informações sobre como remover as versões antigas do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-139">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="6170c-140">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="6170c-140">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="6170c-141">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6170c-141">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="6170c-142">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="6170c-142">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="6170c-143">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-143">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="6170c-144">Pode instalar ou carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion`:</span><span class="sxs-lookup"><span data-stu-id="6170c-144">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="6170c-145">Se tiver mais do que uma versão do módulo instalada, faça o carregamento automático do módulo e carregue a versão mais recente com `Import-Module` por predefinição.</span><span class="sxs-lookup"><span data-stu-id="6170c-145">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="6170c-146">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="6170c-146">Provide feedback</span></span>

<span data-ttu-id="6170c-147">Se encontrar um erro no Azure Powershell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="6170c-147">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="6170c-148">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="6170c-148">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6170c-149">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="6170c-149">Next Steps</span></span>

<span data-ttu-id="6170c-150">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-150">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="6170c-151">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="6170c-151">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
