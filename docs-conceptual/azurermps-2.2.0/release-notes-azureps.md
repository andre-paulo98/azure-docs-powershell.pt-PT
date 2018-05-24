---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 6fe226a2525142f82b894318b0588681bff0e2ef
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2018
---
# <a name="release-notes"></a><span data-ttu-id="9974e-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="9974e-103">Release notes</span></span>

<span data-ttu-id="9974e-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="9974e-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="9974e-105">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="9974e-105">Version 2.2.0</span></span>
* <span data-ttu-id="9974e-106">Computação</span><span class="sxs-lookup"><span data-stu-id="9974e-106">Compute</span></span>
  - <span data-ttu-id="9974e-107">Adição de suporte para consultar o estado de encriptação a partir da extensão AzureDiskEncryptionForLinux</span><span class="sxs-lookup"><span data-stu-id="9974e-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="9974e-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="9974e-108">DataFactory</span></span>
  - <span data-ttu-id="9974e-109">Novo cmdlet adicionado para a listagem de janelas de atividade</span><span class="sxs-lookup"><span data-stu-id="9974e-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="9974e-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="9974e-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="9974e-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="9974e-111">DataLake</span></span>
  - <span data-ttu-id="9974e-112">O parâmetro `Host` foi alterado para `DatabaseHost` e foi adicionado um alias a `Host`</span><span class="sxs-lookup"><span data-stu-id="9974e-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="9974e-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="9974e-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="9974e-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="9974e-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="9974e-115">Adição de suporte para a remoção de ACL e ACL Predefinida</span><span class="sxs-lookup"><span data-stu-id="9974e-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="9974e-116">Adição de suporte para obter e definir permissões sem nome em ficheiros e pastas</span><span class="sxs-lookup"><span data-stu-id="9974e-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="9974e-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9974e-117">KeyVault</span></span>
  - <span data-ttu-id="9974e-118">Adição de suporte para certificados</span><span class="sxs-lookup"><span data-stu-id="9974e-118">Add support for certificates</span></span>
    + <span data-ttu-id="9974e-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="9974e-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="9974e-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="9974e-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="9974e-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="9974e-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="9974e-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="9974e-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="9974e-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="9974e-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="9974e-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="9974e-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="9974e-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="9974e-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="9974e-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="9974e-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="9974e-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="9974e-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="9974e-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="9974e-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="9974e-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="9974e-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="9974e-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="9974e-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="9974e-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="9974e-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="9974e-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="9974e-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="9974e-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="9974e-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="9974e-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="9974e-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="9974e-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="9974e-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="9974e-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="9974e-138">Rede</span><span class="sxs-lookup"><span data-stu-id="9974e-138">Network</span></span>

  - <span data-ttu-id="9974e-139">Novo parâmetro opcional adicionado para a interface de rede ativar/desativar o funcionamento em rede acelerado +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span><span class="sxs-lookup"><span data-stu-id="9974e-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="9974e-140">Ativação de cmdlets do PowerShell da funcionalidade de gateway Ativo-Ativo</span><span class="sxs-lookup"><span data-stu-id="9974e-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="9974e-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9974e-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="9974e-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9974e-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="9974e-143">Novo cmdlet adicionado</span><span class="sxs-lookup"><span data-stu-id="9974e-143">Added new cmdlet</span></span>
    + <span data-ttu-id="9974e-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="9974e-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="9974e-145">Recursos</span><span class="sxs-lookup"><span data-stu-id="9974e-145">Resources</span></span>
  - <span data-ttu-id="9974e-146">Zonas de suporte nos cmdlets de fornecedor e de recursos</span><span class="sxs-lookup"><span data-stu-id="9974e-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="9974e-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="9974e-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="9974e-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="9974e-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="9974e-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="9974e-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="9974e-150">SQL</span><span class="sxs-lookup"><span data-stu-id="9974e-150">Sql</span></span>
  - <span data-ttu-id="9974e-151">Foram adicionados novos cmdlets para a gestão da política de deteção de ameaças de SQL do Azure ao nível do servidor</span><span class="sxs-lookup"><span data-stu-id="9974e-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="9974e-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="9974e-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="9974e-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="9974e-155">Foram adicionados novos cmdlets para suportar a ativação/desativação de GeoBackupPolicy para DataWarehouses do SQL Azure</span><span class="sxs-lookup"><span data-stu-id="9974e-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="9974e-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="9974e-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="9974e-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="9974e-158">Foram adicionados novos cmdlets para as APIs Ações Recomendadas e Assistentes de SQL</span><span class="sxs-lookup"><span data-stu-id="9974e-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="9974e-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="9974e-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="9974e-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="9974e-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="9974e-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="9974e-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="9974e-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="9974e-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="9974e-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="9974e-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="9974e-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="9974e-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="9974e-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="9974e-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="9974e-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="9974e-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="9974e-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="9974e-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="9974e-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="9974e-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="9974e-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="9974e-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="9974e-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="9974e-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
