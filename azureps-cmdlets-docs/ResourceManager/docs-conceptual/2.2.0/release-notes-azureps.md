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
ms.openlocfilehash: 143d92384fd270711378f6741ba59e88c12833d1
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="8f248-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="8f248-103">Release notes</span></span>
<a id="release-notes" class="xliff"></a>

<span data-ttu-id="8f248-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="8f248-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <span data-ttu-id="8f248-105">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="8f248-105">Version 2.2.0</span></span>
<a id="version-220" class="xliff"></a>
* <span data-ttu-id="8f248-106">Computação</span><span class="sxs-lookup"><span data-stu-id="8f248-106">Compute</span></span>
  - <span data-ttu-id="8f248-107">Adição de suporte para consultar o estado de encriptação a partir da extensão AzureDiskEncryptionForLinux</span><span class="sxs-lookup"><span data-stu-id="8f248-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="8f248-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="8f248-108">DataFactory</span></span>
  - <span data-ttu-id="8f248-109">Novo cmdlet adicionado para a listagem de janelas de atividade</span><span class="sxs-lookup"><span data-stu-id="8f248-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="8f248-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="8f248-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="8f248-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="8f248-111">DataLake</span></span>
  - <span data-ttu-id="8f248-112">O parâmetro `Host` foi alterado para `DatabaseHost` e foi adicionado um alias a `Host`</span><span class="sxs-lookup"><span data-stu-id="8f248-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="8f248-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="8f248-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="8f248-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="8f248-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="8f248-115">Adição de suporte para a remoção de ACL e ACL Predefinida</span><span class="sxs-lookup"><span data-stu-id="8f248-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="8f248-116">Adição de suporte para obter e definir permissões sem nome em ficheiros e pastas</span><span class="sxs-lookup"><span data-stu-id="8f248-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="8f248-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8f248-117">KeyVault</span></span>
  - <span data-ttu-id="8f248-118">Adição de suporte para certificados</span><span class="sxs-lookup"><span data-stu-id="8f248-118">Add support for certificates</span></span>
    + <span data-ttu-id="8f248-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="8f248-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="8f248-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="8f248-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="8f248-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="8f248-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="8f248-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="8f248-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="8f248-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="8f248-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="8f248-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="8f248-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="8f248-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="8f248-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="8f248-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="8f248-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="8f248-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="8f248-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="8f248-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="8f248-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="8f248-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="8f248-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="8f248-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="8f248-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="8f248-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="8f248-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="8f248-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="8f248-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="8f248-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="8f248-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="8f248-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="8f248-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="8f248-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="8f248-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="8f248-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="8f248-138">Rede</span><span class="sxs-lookup"><span data-stu-id="8f248-138">Network</span></span>

  - <span data-ttu-id="8f248-139">Novo parâmetro opcional adicionado para a interface de rede ativar/desativar o funcionamento em rede acelerado +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span><span class="sxs-lookup"><span data-stu-id="8f248-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="8f248-140">Ativação de cmdlets do PowerShell da funcionalidade de gateway Ativo-Ativo</span><span class="sxs-lookup"><span data-stu-id="8f248-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="8f248-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="8f248-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="8f248-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="8f248-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="8f248-143">Novo cmdlet adicionado</span><span class="sxs-lookup"><span data-stu-id="8f248-143">Added new cmdlet</span></span>
    + <span data-ttu-id="8f248-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="8f248-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="8f248-145">Recursos</span><span class="sxs-lookup"><span data-stu-id="8f248-145">Resources</span></span>
  - <span data-ttu-id="8f248-146">Zonas de suporte nos cmdlets de fornecedor e de recursos</span><span class="sxs-lookup"><span data-stu-id="8f248-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="8f248-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="8f248-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="8f248-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="8f248-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="8f248-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="8f248-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="8f248-150">SQL</span><span class="sxs-lookup"><span data-stu-id="8f248-150">Sql</span></span>
  - <span data-ttu-id="8f248-151">Foram adicionados novos cmdlets para a gestão da política de deteção de ameaças de SQL do Azure ao nível do servidor</span><span class="sxs-lookup"><span data-stu-id="8f248-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="8f248-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="8f248-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="8f248-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="8f248-155">Foram adicionados novos cmdlets para suportar a ativação/desativação de GeoBackupPolicy para DataWarehouses do SQL Azure</span><span class="sxs-lookup"><span data-stu-id="8f248-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="8f248-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="8f248-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="8f248-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="8f248-158">Foram adicionados novos cmdlets para as APIs Ações Recomendadas e Assistentes de SQL</span><span class="sxs-lookup"><span data-stu-id="8f248-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="8f248-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="8f248-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="8f248-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="8f248-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="8f248-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="8f248-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="8f248-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="8f248-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="8f248-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="8f248-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="8f248-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="8f248-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="8f248-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="8f248-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="8f248-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="8f248-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="8f248-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="8f248-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="8f248-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="8f248-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="8f248-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="8f248-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="8f248-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="8f248-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
