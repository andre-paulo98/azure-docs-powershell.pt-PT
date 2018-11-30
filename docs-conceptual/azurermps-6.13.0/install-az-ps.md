---
title: Instalar o módulo "Az" do Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet no Windows, macOS e Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/26/2018
ms.openlocfilehash: 3d52b18750341f220dc8e10d6bf89796457c5a10
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/29/2018
ms.locfileid: "52588184"
---
# <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="a5477-103">Instalar o módulo "Az" do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a5477-103">Install the Azure PowerShell 'Az' module</span></span>

<span data-ttu-id="a5477-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="a5477-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="a5477-105">Estas instruções funcionam nas plataformas Windows, macOS e Linux.</span><span class="sxs-lookup"><span data-stu-id="a5477-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="a5477-106">Para a versão de pré-visualização do Az, não são suportados outros métodos de instalação.</span><span class="sxs-lookup"><span data-stu-id="a5477-106">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="a5477-107">Requisitos</span><span class="sxs-lookup"><span data-stu-id="a5477-107">Requirements</span></span>

<span data-ttu-id="a5477-108">O Azure PowerShell funciona com o PowerShell 5.x no Windows ou no PowerShell 6.x em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="a5477-108">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="a5477-109">Para verificar a versão do PowerShell em execução na sua máquina, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="a5477-109">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="a5477-110">Se tiver uma versão desatualizada ou precisar de instalar o PowerShell, veja [Instalar várias versões do PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="a5477-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="a5477-111">As informações sobre a instalação da sua plataforma estão associadas a essa página.</span><span class="sxs-lookup"><span data-stu-id="a5477-111">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="a5477-112">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a5477-112">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="a5477-113">Pode ter ambos os módulos `AzureRM` e `Az` instalados em simultâneo.</span><span class="sxs-lookup"><span data-stu-id="a5477-113">You can have both the `AzureRM` and `Az` modules installed at the same time.</span></span> <span data-ttu-id="a5477-114">Se tiver ambos os módulos instalados, __não ative os aliases__.</span><span class="sxs-lookup"><span data-stu-id="a5477-114">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="a5477-115">Ativar os aliases causa conflitos entre os cmdlets `AzureRM` e os aliases de comando `Az`, o que pode causar comportamentos inesperados.</span><span class="sxs-lookup"><span data-stu-id="a5477-115">Enabling aliases will cause conflicts between `AzureRM` cmdlets and `Az` command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="a5477-116">É recomendado que antes de instalar o módulo `Az`, desinstale `AzureRM`.</span><span class="sxs-lookup"><span data-stu-id="a5477-116">It's recommended that before installing the `Az` module, you uninstall `AzureRM`.</span></span> <span data-ttu-id="a5477-117">Pode sempre desinstalar `AzureRM` ou ativar aliases a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="a5477-117">You can always uninstall `AzureRM` or enable aliases at any time.</span></span> <span data-ttu-id="a5477-118">Para instruções de desinstalação, veja [Desinstalar o módulo do Azure PowerShell (AzureRM)](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="a5477-118">For uninstall instructions, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span> 

<span data-ttu-id="a5477-119">Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a5477-119">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="a5477-120">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):</span><span class="sxs-lookup"><span data-stu-id="a5477-120">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="a5477-121">Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.</span><span class="sxs-lookup"><span data-stu-id="a5477-121">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="a5477-122">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="a5477-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="a5477-123">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="a5477-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="a5477-124">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="a5477-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="a5477-125">O módulo `Az` é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a5477-125">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="a5477-126">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="a5477-126">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="a5477-127">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="a5477-127">Sign in</span></span>

<span data-ttu-id="a5477-128">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="a5477-128">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="a5477-129">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="a5477-129">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="a5477-130">Devido à forma como o módulo está estruturado, esta operação pode demorar alguns segundos.</span><span class="sxs-lookup"><span data-stu-id="a5477-130">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="a5477-131">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="a5477-131">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="a5477-132">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="a5477-132">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="a5477-133">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a5477-133">Update the Azure PowerShell module</span></span>

<span data-ttu-id="a5477-134">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="a5477-134">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="a5477-135">Este comando __não__ desinstala as versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="a5477-135">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="a5477-136">Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="a5477-136">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="a5477-137">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a5477-137">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="a5477-138">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a5477-138">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="a5477-139">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="a5477-139">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="a5477-140">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="a5477-140">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="a5477-141">Pode carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion` com `Install-Module` e `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="a5477-141">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` and `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="a5477-142">Se tiver mais do que uma versão do módulo instalada, a versão mais recente é carregada por predefinição.</span><span class="sxs-lookup"><span data-stu-id="a5477-142">If you have more than one version of the module installed, the latest version is loaded by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="a5477-143">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="a5477-143">Provide feedback</span></span>

<span data-ttu-id="a5477-144">Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="a5477-144">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="a5477-145">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="a5477-145">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a5477-146">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="a5477-146">Next Steps</span></span>

<span data-ttu-id="a5477-147">Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.</span><span class="sxs-lookup"><span data-stu-id="a5477-147">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
