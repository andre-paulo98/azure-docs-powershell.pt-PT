---
title: Instalar o Azure PowerShell com um MSI
description: Como instalar o Azure PowerShell sem o PowerShellGet utilizar um MSI
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/22/2019
ms.openlocfilehash: 1bae6879dcf3cd56f9a8d6400bcd516e0cbf6a19
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84121650"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="1d4d0-103">Instalar o Azure PowerShell no Windows com o MSI</span><span class="sxs-lookup"><span data-stu-id="1d4d0-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="1d4d0-104">Este artigo explica como instalar o Azure PowerShell no Windows com um Instalador do MSI.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span> <span data-ttu-id="1d4d0-105">O instalador MSI é fornecido para ambientes onde a Galeria do PowerShell pode ser bloqueada por uma firewall ou onde for necessário um instalador offline.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-105">The MSI installer is provided for environments where the PowerShell Gallery may be blocked by a firewall, or an offline installer is needed.</span></span> <span data-ttu-id="1d4d0-106">A forma recomendada para instalar o Azure PowerShell é através do PowerShellGet.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-106">The recommended way to install Azure PowerShell is with PowerShellGet.</span></span> <span data-ttu-id="1d4d0-107">Para obter instruções sobre como utilizar o PowerShellGet para instalar o Azure PowerShell, veja [Instalar o Azure PowerShell com o PowerShellGet](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-az-ps.md).</span></span>

## <a name="requirements"></a><span data-ttu-id="1d4d0-108">Requisitos</span><span class="sxs-lookup"><span data-stu-id="1d4d0-108">Requirements</span></span>

<span data-ttu-id="1d4d0-109">O instalador MSI no Windows foi criado para instalar o Azure PowerShell apenas para o PowerShell 5.1.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-109">The MSI installer on Windows is designed to install Azure PowerShell for PowerShell 5.1 only.</span></span> <span data-ttu-id="1d4d0-110">Para a instalação em plataformas que não sejam do Windows ou versões posteriores do PowerShell, utilize a opção [Instalar com o PowerShellGet](install-az-ps.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-110">For installation on non-Windows platforms or later versions of PowerShell, [Install with PowerShellGet](install-az-ps.md).</span></span> <span data-ttu-id="1d4d0-111">Para consultar a sua versão do PowerShell, execute o comando:</span><span class="sxs-lookup"><span data-stu-id="1d4d0-111">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="1d4d0-112">Para utilizar o Azure PowerShell no PowerShell 5.1:</span><span class="sxs-lookup"><span data-stu-id="1d4d0-112">To use Azure PowerShell in PowerShell 5.1, you need to:</span></span>

1. <span data-ttu-id="1d4d0-113">Atualize para o [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell) se for necessário.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-113">Update to [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="1d4d0-114">Se estiver no Windows 10, já tem o PowerShell 5.1 instalado.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-114">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="1d4d0-115">Instale o [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-115">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="1d4d0-116">Instalar ou atualizar no Windows com o Pacote MSI</span><span class="sxs-lookup"><span data-stu-id="1d4d0-116">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="1d4d0-117">O pacote MSI para o Azure PowerShell está disponível a partir do [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v1.8.0-April2019).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-117">The MSI package for Azure PowerShell is available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v1.8.0-April2019).</span></span> <span data-ttu-id="1d4d0-118">Se tiver instalado versões anteriores do Azure PowerShell com o MSI, o instalador remove-as automaticamente.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-118">If you have installed earlier versions of Azure PowerShell using the MSI, the installer automatically removes them.</span></span> <span data-ttu-id="1d4d0-119">O pacote do MSI instala os módulos em `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-119">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span>

<span data-ttu-id="1d4d0-120">Para começar a trabalhar com o Azure PowerShell, inicie sessão com as suas credenciais do Azure.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-120">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="1d4d0-121">Se tiver desativado o carregamento automático do módulo, tem de importar o módulo manualmente com `Import-Module Az`.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-121">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="1d4d0-122">Devido à forma como o módulo está estruturado, esta operação pode demorar um minuto.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-122">Because of the way the module is structured, this can take up to a minute.</span></span>

<span data-ttu-id="1d4d0-123">Terá de repetir este passo para cada nova sessão do PowerShell que iniciar.</span><span class="sxs-lookup"><span data-stu-id="1d4d0-123">You'll need to repeat this step for every new PowerShell session you start.</span></span> <span data-ttu-id="1d4d0-124">Para saber como manter o início de sessão do Azure nas sessões do PowerShell, veja [Manter as credenciais do utilizador nas sessões do PowerShell](context-persistence.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-124">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="1d4d0-125">Enviar comentários</span><span class="sxs-lookup"><span data-stu-id="1d4d0-125">Provide feedback</span></span>

<span data-ttu-id="1d4d0-126">Se encontrar um erro no Azure PowerShell, [registe um problema no GitHub](https://github.com/Azure/azure-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-126">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="1d4d0-127">Para enviar comentários a partir da linha de comandos, experimente o cmdlet [Send-Feedback](/powershell/module/az.accounts/send-feedback).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-127">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1d4d0-128">Passos Seguintes</span><span class="sxs-lookup"><span data-stu-id="1d4d0-128">Next Steps</span></span>

<span data-ttu-id="1d4d0-129">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-129">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="1d4d0-130">Se estiver familiarizado com o Azure PowerShell e precisar de migrar do AzureRM, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).</span><span class="sxs-lookup"><span data-stu-id="1d4d0-130">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
