---
title: "Registo de alterações do Azure PowerShell | Microsoft Docs"
description: "Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente."
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 04f89e8d47d0825d46cb1b8817efbcc0cafa0acd
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/03/2017
---
# <a name="release-notes"></a><span data-ttu-id="81d53-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="81d53-103">Release notes</span></span>

<span data-ttu-id="81d53-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="81d53-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-380"></a><span data-ttu-id="81d53-105">Versão 3.8.0</span><span class="sxs-lookup"><span data-stu-id="81d53-105">Version 3.8.0</span></span>
* <span data-ttu-id="81d53-106">Computação</span><span class="sxs-lookup"><span data-stu-id="81d53-106">Compute</span></span>
  - <span data-ttu-id="81d53-107">Correção de erros nos cmdlets Get-*, para permitir a obtenção de várias páginas de dados (mais de 120 itens)</span><span class="sxs-lookup"><span data-stu-id="81d53-107">Fix bug in Get-* cmdlets, to allow retrieving multiple pages of data (more than 120 items)</span></span>
* <span data-ttu-id="81d53-108">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="81d53-108">DataLakeAnalytics</span></span>
  - <span data-ttu-id="81d53-109">Correção da ajuda de alguns comandos para ter o texto e os exemplos adequados.</span><span class="sxs-lookup"><span data-stu-id="81d53-109">Fix help for some commands to have the proper verbage and examples.</span></span>
* <span data-ttu-id="81d53-110">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="81d53-110">DataLakeStore</span></span>
  - <span data-ttu-id="81d53-111">Adição de suporte relativo à parte inicial e final ao cmdlet `Get-AzureRMDataLakeStoreItemContent`.</span><span class="sxs-lookup"><span data-stu-id="81d53-111">Add support for head and tail to the `Get-AzureRMDataLakeStoreItemContent` cmdlet.</span></span> <span data-ttu-id="81d53-112">Isto permite a apresentação das linhas delimitadas por nova linha N inicial ou N final.</span><span class="sxs-lookup"><span data-stu-id="81d53-112">This enables returning the top N or last N new line delimited rows to be displayed.</span></span>
* <span data-ttu-id="81d53-113">HDInsight</span><span class="sxs-lookup"><span data-stu-id="81d53-113">HDInsight</span></span>
  - <span data-ttu-id="81d53-114">Foi adicionado suporte para o tipo de cluster RServer</span><span class="sxs-lookup"><span data-stu-id="81d53-114">Added support for RServer cluster type</span></span>
    + <span data-ttu-id="81d53-115">O tamanho da VM Edgenode pode ser especificado para o cluster RServer em New-AzureRmHDInsightCluster ou New-AzureRmHDInsightClusterConfig</span><span class="sxs-lookup"><span data-stu-id="81d53-115">Edgenode VM size can be specified for RServer cluster in New-AzureRmHDInsightCluster or New-AzureRmHDInsightClusterConfig</span></span>
    + <span data-ttu-id="81d53-116">RServer é agora uma opção de configuração em Add-AzureRmHDInsightConfigValues.</span><span class="sxs-lookup"><span data-stu-id="81d53-116">RServer is now a configuration option in Add-AzureRmHDInsightConfigValues.</span></span> <span data-ttu-id="81d53-117">Permite definir o sinalizador de RStudio para indicar que a instalação do R Studio deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="81d53-117">It allows for RStudio flag to be set to indicate that R Studio installation should be done.</span></span>
* <span data-ttu-id="81d53-118">LogicApp</span><span class="sxs-lookup"><span data-stu-id="81d53-118">LogicApp</span></span>
  - <span data-ttu-id="81d53-119">Os cmdlets Set-AzureRmIntegrationAccountSchema e Set-AzureRmIntegrationAccountMap foram corrigidos para o problema de contentlink (content e contentlink estavam definidos, o que resultava numa falha de atualização).</span><span class="sxs-lookup"><span data-stu-id="81d53-119">Set-AzureRmIntegrationAccountSchema and Set-AzureRmIntegrationAccountMap cmdlets are fixed for the contentlink issue(Both content and contentlink were set resulting in update failure).</span></span>
* <span data-ttu-id="81d53-120">Rede</span><span class="sxs-lookup"><span data-stu-id="81d53-120">Network</span></span>
  - <span data-ttu-id="81d53-121">Foi adicionado suporte para novas funcionalidades de firewall da aplicação Web aos Gateways de Aplicação</span><span class="sxs-lookup"><span data-stu-id="81d53-121">Added support for new web application firewall features to Application Gateways</span></span>
    + <span data-ttu-id="81d53-122">New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig adicionado</span><span class="sxs-lookup"><span data-stu-id="81d53-122">Added New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig</span></span>
    + <span data-ttu-id="81d53-123">Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets) adicionado</span><span class="sxs-lookup"><span data-stu-id="81d53-123">Added Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets)</span></span>
    + <span data-ttu-id="81d53-124">New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration atualizado: parâmetro adicionado -RuleSetType -RuleSetVersion e -DisabledRuleGroups</span><span class="sxs-lookup"><span data-stu-id="81d53-124">Updated New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
    + <span data-ttu-id="81d53-125">Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration atualizado: parâmetro adicionado -RuleSetType -RuleSetVersion e -DisabledRuleGroups</span><span class="sxs-lookup"><span data-stu-id="81d53-125">Updated Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
  - <span data-ttu-id="81d53-126">Foi adicionado suporte para políticas IPSec às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="81d53-126">Added support for IPSec policies to Virtual Network Gateway Connections</span></span>
  - <span data-ttu-id="81d53-127">New-AzureRmIpsecPolicy adicionado</span><span class="sxs-lookup"><span data-stu-id="81d53-127">Added New-AzureRmIpsecPolicy</span></span>
  - <span data-ttu-id="81d53-128">New-AzureRmVirtualNetworkGatewayConnection atualizado: parâmetro adicionado -IpsecPolicies e -UsePolicyBasedTrafficSelectors</span><span class="sxs-lookup"><span data-stu-id="81d53-128">Updated New-AzureRmVirtualNetworkGatewayConnection: Added parameter -IpsecPolicies and -UsePolicyBasedTrafficSelectors</span></span>
* <span data-ttu-id="81d53-129">Perfil</span><span class="sxs-lookup"><span data-stu-id="81d53-129">Profile</span></span>
  - <span data-ttu-id="81d53-130">*Obsoleto*: o nome de Save-AzureRmProfile foi mudado para Save-AzureRmContext; existe um alias para o nome antigo do cmdlet; o alias será removido na próxima versão.</span><span class="sxs-lookup"><span data-stu-id="81d53-130">*Obsolete*: Save-AzureRmProfile is renamed to Save-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="81d53-131">*Obsoleto*: o nome de Select-AzureRmProfile foi mudado para Import-AzureRmContext; existe um alias para o nome antigo do cmdlet; o alias será removido na próxima versão.</span><span class="sxs-lookup"><span data-stu-id="81d53-131">*Obsolete*: Select-AzureRmProfile is renamed to Import-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="81d53-132">Os tipos de saída PSAzureContext e PSAzureProfile dos cmdlets de perfil vão ser alterados na próxima versão.</span><span class="sxs-lookup"><span data-stu-id="81d53-132">The PSAzureContext and PSAzureProfile output types of profile cmdlets will be changed in the next release.</span></span>
  - <span data-ttu-id="81d53-133">O cmdlet Save-AzureRmContext não terá qualquer OutputType na próxima versão.</span><span class="sxs-lookup"><span data-stu-id="81d53-133">The Save-AzureRmContext cmdlet will have no OutputType in the next release.</span></span>
  - <span data-ttu-id="81d53-134">Correção de erro no código comum do cmdlet para utilizar o algoritmo compatível com FIPS para hashes de dados: https://github.com/Azure/azure-powershell/issues/3651</span><span class="sxs-lookup"><span data-stu-id="81d53-134">Fix bug in cmdlet common code to use FIPS-compliant algorithm for data hashes: https://github.com/Azure/azure-powershell/issues/3651</span></span>
* <span data-ttu-id="81d53-135">SQL</span><span class="sxs-lookup"><span data-stu-id="81d53-135">Sql</span></span>
  - <span data-ttu-id="81d53-136">Correções de erros no Cmdlets de Grupo de Ativação Pós-falha do Azure</span><span class="sxs-lookup"><span data-stu-id="81d53-136">Bug fixes on Azure Failover Group Cmdlets</span></span>
  - <span data-ttu-id="81d53-137">Correção para a consulta de operações</span><span class="sxs-lookup"><span data-stu-id="81d53-137">Fix for operation polling</span></span>
  - <span data-ttu-id="81d53-138">Correção do valor GracePeriodWithDataLossHour ao definir FailoverPolicy como Manual</span><span class="sxs-lookup"><span data-stu-id="81d53-138">Fix GracePeriodWithDataLossHour value when setting FailoverPolicy to Manual</span></span>
* <span data-ttu-id="81d53-139">TrafficManager</span><span class="sxs-lookup"><span data-stu-id="81d53-139">TrafficManager</span></span>
  - <span data-ttu-id="81d53-140">Suporte para o método de encaminhamento de tráfego Geográfico</span><span class="sxs-lookup"><span data-stu-id="81d53-140">Support for the Geographic traffic routing method</span></span>
    + <span data-ttu-id="81d53-141">Novo valor 'Geographic' para o parâmetro TrafficRoutingMethod de New-AzureRmTrafficManagerProfile</span><span class="sxs-lookup"><span data-stu-id="81d53-141">New value 'Geographic' for the TrafficRoutingMethod parameter of New-AzureRmTrafficManagerProfile</span></span>
    + <span data-ttu-id="81d53-142">Novo parâmetro GeoMapping para New-AzureRmTrafficManagerEndpoint e Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="81d53-142">New parameter 'GeoMapping' for the New-AzureRmTrafficManagerEndpoint and Add-AzureRmTrafficManagerEndpointConfig</span></span>
    + <span data-ttu-id="81d53-143">Correção da tubagem para Get-AzureRmTrafficManagerProfile quando devolve um conjunto de perfis</span><span class="sxs-lookup"><span data-stu-id="81d53-143">Fix piping for Get-AzureRmTrafficManagerProfile when it returns a collection of profiles</span></span>
* <span data-ttu-id="81d53-144">ServiceManagement</span><span class="sxs-lookup"><span data-stu-id="81d53-144">ServiceManagement</span></span>
  - <span data-ttu-id="81d53-145">Restart-AzureVM: parâmetro InitiateMaintenance adicionado para executar a manutenção durante o reinício da VM.</span><span class="sxs-lookup"><span data-stu-id="81d53-145">Restart-AzureVM: Added InitiateMaintenance parameter for performing maintenance during VM restart.</span></span>
  - <span data-ttu-id="81d53-146">Get-AzureVM: campo de Estado de Manutenção adicionado.</span><span class="sxs-lookup"><span data-stu-id="81d53-146">Get-AzureVM: Added Maintenance Status field.</span></span>
  - <span data-ttu-id="81d53-147">Novos cmdlets adicionados para suportar a atualização do cofre dos Serviços de Recuperação</span><span class="sxs-lookup"><span data-stu-id="81d53-147">Added new cmdlets to support Recovery Services vault upgrade</span></span>
    + <span data-ttu-id="81d53-148">Test-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="81d53-148">Test-AzureRecoveryServicesVaultUpgrade</span></span>
    + <span data-ttu-id="81d53-149">Invoke-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="81d53-149">Invoke-AzureRecoveryServicesVaultUpgrade</span></span>