---
title: Instalar o Azure PowerShell com o PowerShellGet
description: Como instalar o Azure PowerShell com o PowerShellGet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: c4af07816aaa6713d67e3349a45880f8cc22c80a
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574503"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="f31ef-103">Instalar o Azure PowerShell com o PowerShellGet</span><span class="sxs-lookup"><span data-stu-id="f31ef-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="f31ef-104">Este artigo mostra-lhe como instalar os módulos do Azure PowerShell com o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="f31ef-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="f31ef-105">Para a versão de pré-visualização do Az, não são suportados outros métodos de instalação.</span><span class="sxs-lookup"><span data-stu-id="f31ef-105">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="f31ef-106">Requisitos</span><span class="sxs-lookup"><span data-stu-id="f31ef-106">Requirements</span></span>

<span data-ttu-id="f31ef-107">O Azure PowerShell funciona com o PowerShell 5.x no Windows ou no PowerShell 6.x em qualquer plataforma.</span><span class="sxs-lookup"><span data-stu-id="f31ef-107">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="f31ef-108">Para verificar a versão do PowerShell em execução na sua máquina, execute o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="f31ef-108">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="f31ef-109">Se tiver uma versão desatualizada ou precisar de instalar o PowerShell, veja [Instalar várias versões do PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="f31ef-109">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="f31ef-110">As informações sobre a instalação da sua plataforma estão associadas a essa página.</span><span class="sxs-lookup"><span data-stu-id="f31ef-110">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="f31ef-111">Instalar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f31ef-111">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="f31ef-112">Não deve ter os módulos `AzureRM` e `Az` instalados num sistema ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="f31ef-112">You shouldn't have both the `AzureRM` and `Az` modules installed on a system at the same time.</span></span> <span data-ttu-id="f31ef-113">Para instalar o módulo `Az`, o `AzureRM` tem de ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="f31ef-113">In order to install the `Az` module, `AzureRM` must be uninstalled.</span></span> <span data-ttu-id="f31ef-114">Para obter instruções sobre como fazê-lo, veja [Desinstalar o módulo do Azure PowerShell (AzureRM)](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="f31ef-114">For instructions on how to do that, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="f31ef-115">Para instalar módulo num âmbito global, precisa de privilégios elevados para instalar módulos da Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f31ef-115">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="f31ef-116">Para instalar o Azure PowerShell, execute o seguinte comando numa sessão elevada ("Executar como Administrador" no Windows, ou com privilégios de superutilizador no macOS ou Linux):</span><span class="sxs-lookup"><span data-stu-id="f31ef-116">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="f31ef-117">Se não tiver acesso a privilégios de administrador, pode instalar para o utilizador atual, ao adicionar o argumento `-Scope`.</span><span class="sxs-lookup"><span data-stu-id="f31ef-117">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="f31ef-118">Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="f31ef-118">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="f31ef-119">Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:</span><span class="sxs-lookup"><span data-stu-id="f31ef-119">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="f31ef-120">Responda `Yes` ou `Yes to All` para continuar com a instalação.</span><span class="sxs-lookup"><span data-stu-id="f31ef-120">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="f31ef-121">O módulo `Az` é um módulo de rollup para os cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f31ef-121">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="f31ef-122">A instalação do mesmo transfere todos os módulos disponíveis do Azure Resource Manager e disponibiliza os respetivos cmdlets para utilização.</span><span class="sxs-lookup"><span data-stu-id="f31ef-122">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="f31ef-123">Iniciar sessão</span><span class="sxs-lookup"><span data-stu-id="f31ef-123">Sign in</span></span>

<span data-ttu-id="f31ef-124">Para começar a utilizar o Azure PowerShell, precisa de carregar `Az` para a sua sessão atual do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="f31ef-124">To start working with Azure PowerShell, you need to load `Az` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

<span data-ttu-id="f31ef-125">Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada.</span><span class="sxs-lookup"><span data-stu-id="f31ef-125">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="f31ef-126">A importação automática do módulo `Az` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).</span><span class="sxs-lookup"><span data-stu-id="f31ef-126">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="f31ef-127">Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="f31ef-127">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="f31ef-128">Atualizar o módulo do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f31ef-128">Update the Azure PowerShell module</span></span>

<span data-ttu-id="f31ef-129">Pode atualizar a sua instalação do Azure PowerShell ao executar [Update-Module](/powershell/module/powershellget/update-module).</span><span class="sxs-lookup"><span data-stu-id="f31ef-129">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="f31ef-130">Este comando __não__ desinstala as versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="f31ef-130">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="f31ef-131">Se pretende remover as versões anteriores do Azure PowerShell do seu sistema, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="f31ef-131">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="f31ef-132">Utilizar várias versões do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="f31ef-132">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="f31ef-133">Pode instalar mais de uma versão do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f31ef-133">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="f31ef-134">Para verificar se tem várias versões do Azure PowerShell instaladas, utilize o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="f31ef-134">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="f31ef-135">Para remover uma versão do Azure PowerShell, veja [Desinstalar o módulo do Azure PowerShell](uninstall-azurerm-ps.md).</span><span class="sxs-lookup"><span data-stu-id="f31ef-135">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="f31ef-136">Pode carregar uma versão específica do módulo `Az` com o argumento `-RequiredVersion` com `Install-Module` ou `Import-Module`:</span><span class="sxs-lookup"><span data-stu-id="f31ef-136">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` or `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="f31ef-137">Se tiver mais de uma versão do módulo instalado, a versão mais recente é carregada por predefinição ao importar.</span><span class="sxs-lookup"><span data-stu-id="f31ef-137">If you have more than one version of the module installed, the latest version is loaded by default when importing.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="f31ef-138">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="f31ef-138">Provide feedback</span></span>

<span data-ttu-id="f31ef-139">Se encontrar um erro ao utilizar o Azure Powershell, [registe um erro no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="f31ef-139">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="f31ef-140">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.profile/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="f31ef-140">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f31ef-141">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="f31ef-141">Next Steps</span></span>

<span data-ttu-id="f31ef-142">Para começar a utilizar o Azure PowerShell, veja [Introdução ao Azure PowerShell](get-started-azureps.md) para saber mais sobre o módulo e os respetivos recursos.</span><span class="sxs-lookup"><span data-stu-id="f31ef-142">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>