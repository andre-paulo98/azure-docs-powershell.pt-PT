---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: ca25f3c66f8e8f4c64fc04275da2bd28e32d2f6c
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/08/2018
ms.locfileid: "34854618"
---
# <a name="release-notes"></a><span data-ttu-id="3c7a6-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="3c7a6-103">Release notes</span></span>

<span data-ttu-id="3c7a6-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="3c7a6-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-220"></a><span data-ttu-id="3c7a6-105">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="3c7a6-105">Version 2.2.0</span></span>
* <span data-ttu-id="3c7a6-106">Computação</span><span class="sxs-lookup"><span data-stu-id="3c7a6-106">Compute</span></span>
  - <span data-ttu-id="3c7a6-107">Adição de suporte para consultar o estado de encriptação a partir da extensão AzureDiskEncryptionForLinux</span><span class="sxs-lookup"><span data-stu-id="3c7a6-107">Add support for querying encryption status from the AzureDiskEncryptionForLinux extension</span></span>
* <span data-ttu-id="3c7a6-108">DataFactory</span><span class="sxs-lookup"><span data-stu-id="3c7a6-108">DataFactory</span></span>
  - <span data-ttu-id="3c7a6-109">Novo cmdlet adicionado para a listagem de janelas de atividade</span><span class="sxs-lookup"><span data-stu-id="3c7a6-109">Added new cmdlet for listing activity windows</span></span>
    + <span data-ttu-id="3c7a6-110">Get-AzureRmDataFactoryActivityWindow</span><span class="sxs-lookup"><span data-stu-id="3c7a6-110">Get-AzureRmDataFactoryActivityWindow</span></span>
* <span data-ttu-id="3c7a6-111">DataLake</span><span class="sxs-lookup"><span data-stu-id="3c7a6-111">DataLake</span></span>
  - <span data-ttu-id="3c7a6-112">O parâmetro `Host` foi alterado para `DatabaseHost` e foi adicionado um alias a `Host`</span><span class="sxs-lookup"><span data-stu-id="3c7a6-112">Changed parameter `Host` to `DatabaseHost` and added alias to `Host`</span></span>
    + <span data-ttu-id="3c7a6-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="3c7a6-113">New-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
    + <span data-ttu-id="3c7a6-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span><span class="sxs-lookup"><span data-stu-id="3c7a6-114">Set-AzureRmDataLakeAnalyticsCatalogSecret</span></span>
  - <span data-ttu-id="3c7a6-115">Adição de suporte para a remoção de ACL e ACL Predefinida</span><span class="sxs-lookup"><span data-stu-id="3c7a6-115">Add support for ACL and Default ACL removal</span></span>
  - <span data-ttu-id="3c7a6-116">Adição de suporte para obter e definir permissões sem nome em ficheiros e pastas</span><span class="sxs-lookup"><span data-stu-id="3c7a6-116">Add support for getting and setting unnamed permissions on files and folders</span></span>
* <span data-ttu-id="3c7a6-117">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c7a6-117">KeyVault</span></span>
  - <span data-ttu-id="3c7a6-118">Adição de suporte para certificados</span><span class="sxs-lookup"><span data-stu-id="3c7a6-118">Add support for certificates</span></span>
    + <span data-ttu-id="3c7a6-119">Add-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="3c7a6-119">Add-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="3c7a6-120">Add-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="3c7a6-120">Add-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="3c7a6-121">Get-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="3c7a6-121">Get-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="3c7a6-122">Get-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="3c7a6-122">Get-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="3c7a6-123">Get-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="3c7a6-123">Get-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="3c7a6-124">Get-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="3c7a6-124">Get-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="3c7a6-125">Get-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-125">Get-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="3c7a6-126">Import-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="3c7a6-126">Import-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="3c7a6-127">New-AzureKeyVaultCertificateAdministratorDetails</span><span class="sxs-lookup"><span data-stu-id="3c7a6-127">New-AzureKeyVaultCertificateAdministratorDetails</span></span>
    + <span data-ttu-id="3c7a6-128">New-AzureKeyVaultCertificateOrganizationDetails</span><span class="sxs-lookup"><span data-stu-id="3c7a6-128">New-AzureKeyVaultCertificateOrganizationDetails</span></span>
    + <span data-ttu-id="3c7a6-129">New-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-129">New-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="3c7a6-130">Remove-AzureKeyVaultCertificate</span><span class="sxs-lookup"><span data-stu-id="3c7a6-130">Remove-AzureKeyVaultCertificate</span></span>
    + <span data-ttu-id="3c7a6-131">Remove-AzureKeyVaultCertificateContact</span><span class="sxs-lookup"><span data-stu-id="3c7a6-131">Remove-AzureKeyVaultCertificateContact</span></span>
    + <span data-ttu-id="3c7a6-132">Remove-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="3c7a6-132">Remove-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="3c7a6-133">Remove-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="3c7a6-133">Remove-AzureKeyVaultCertificateOperation</span></span>
    + <span data-ttu-id="3c7a6-134">Set-AzureKeyVaultCertificateAttribute</span><span class="sxs-lookup"><span data-stu-id="3c7a6-134">Set-AzureKeyVaultCertificateAttribute</span></span>
    + <span data-ttu-id="3c7a6-135">Set-AzureKeyVaultCertificateIssuer</span><span class="sxs-lookup"><span data-stu-id="3c7a6-135">Set-AzureKeyVaultCertificateIssuer</span></span>
    + <span data-ttu-id="3c7a6-136">Set-AzureKeyVaultCertificatePolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-136">Set-AzureKeyVaultCertificatePolicy</span></span>
    + <span data-ttu-id="3c7a6-137">Stop-AzureKeyVaultCertificateOperation</span><span class="sxs-lookup"><span data-stu-id="3c7a6-137">Stop-AzureKeyVaultCertificateOperation</span></span>
* <span data-ttu-id="3c7a6-138">Rede</span><span class="sxs-lookup"><span data-stu-id="3c7a6-138">Network</span></span>

  - <span data-ttu-id="3c7a6-139">Novo parâmetro opcional adicionado para a interface de rede ativar/desativar o funcionamento em rede acelerado +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span><span class="sxs-lookup"><span data-stu-id="3c7a6-139">New switch parameter added for network interface to enable/disable accelerated networking +New-AzureRmNetworkInterface -EnableAcceleratedNetworking</span></span>
  - <span data-ttu-id="3c7a6-140">Ativação de cmdlets do PowerShell da funcionalidade de gateway Ativo-Ativo</span><span class="sxs-lookup"><span data-stu-id="3c7a6-140">Enable Active-Active gateway feature PowerShell cmdlets</span></span>
    + <span data-ttu-id="3c7a6-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="3c7a6-141">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
    + <span data-ttu-id="3c7a6-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="3c7a6-142">Remove-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="3c7a6-143">Novo cmdlet adicionado</span><span class="sxs-lookup"><span data-stu-id="3c7a6-143">Added new cmdlet</span></span>
    + <span data-ttu-id="3c7a6-144">Test-AzureRmPrivateIpAddressAvailability</span><span class="sxs-lookup"><span data-stu-id="3c7a6-144">Test-AzureRmPrivateIpAddressAvailability</span></span>
* <span data-ttu-id="3c7a6-145">Recursos</span><span class="sxs-lookup"><span data-stu-id="3c7a6-145">Resources</span></span>
  - <span data-ttu-id="3c7a6-146">Zonas de suporte nos cmdlets de fornecedor e de recursos</span><span class="sxs-lookup"><span data-stu-id="3c7a6-146">Support zones in provider and resource cmdlets</span></span>
    + <span data-ttu-id="3c7a6-147">Get-AzureRmProvider</span><span class="sxs-lookup"><span data-stu-id="3c7a6-147">Get-AzureRmProvider</span></span>
    + <span data-ttu-id="3c7a6-148">New-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="3c7a6-148">New-AzureRmResource</span></span>
    + <span data-ttu-id="3c7a6-149">Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="3c7a6-149">Set-AzureRmResource</span></span>
* <span data-ttu-id="3c7a6-150">SQL</span><span class="sxs-lookup"><span data-stu-id="3c7a6-150">Sql</span></span>
  - <span data-ttu-id="3c7a6-151">Foram adicionados novos cmdlets para a gestão da política de deteção de ameaças de SQL do Azure ao nível do servidor</span><span class="sxs-lookup"><span data-stu-id="3c7a6-151">Added new cmdlets for Azure SQL threat detection policy management at server level</span></span>
    + <span data-ttu-id="3c7a6-152">Get-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-152">Get-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="3c7a6-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-153">Remove-AzureRmSqlServerThreatDetectionPolicy</span></span>
    + <span data-ttu-id="3c7a6-154">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-154">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
  - <span data-ttu-id="3c7a6-155">Foram adicionados novos cmdlets para suportar a ativação/desativação de GeoBackupPolicy para DataWarehouses do SQL Azure</span><span class="sxs-lookup"><span data-stu-id="3c7a6-155">Added new cmdlets to support enabling/disabling GeoBackupPolicy for Sql Azure DataWarehouses</span></span>
    + <span data-ttu-id="3c7a6-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-156">Get-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
    + <span data-ttu-id="3c7a6-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span><span class="sxs-lookup"><span data-stu-id="3c7a6-157">Set-AzureRmSqlDatabaseGeoBackupPolicy</span></span>
  - <span data-ttu-id="3c7a6-158">Foram adicionados novos cmdlets para as APIs Ações Recomendadas e Assistentes de SQL</span><span class="sxs-lookup"><span data-stu-id="3c7a6-158">Added new cmdlets for Azure Sql Advisors and Recommended Actions APIs</span></span>
    + <span data-ttu-id="3c7a6-159">Get-AzureRmSqlDatabaseAdvisor</span><span class="sxs-lookup"><span data-stu-id="3c7a6-159">Get-AzureRmSqlDatabaseAdvisor</span></span>
    + <span data-ttu-id="3c7a6-160">Get-AzureRmSqlElasticPoolAdvisor</span><span class="sxs-lookup"><span data-stu-id="3c7a6-160">Get-AzureRmSqlElasticPoolAdvisor</span></span>
    + <span data-ttu-id="3c7a6-161">Get-AzureRmSqlServerAdvisor</span><span class="sxs-lookup"><span data-stu-id="3c7a6-161">Get-AzureRmSqlServerAdvisor</span></span>
    + <span data-ttu-id="3c7a6-162">Get-AzureRmSqlDatabaseRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="3c7a6-162">Get-AzureRmSqlDatabaseRecommendedActions</span></span>
    + <span data-ttu-id="3c7a6-163">Get-AzureRmSqlElasticPoolRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="3c7a6-163">Get-AzureRmSqlElasticPoolRecommendedActions</span></span>
    + <span data-ttu-id="3c7a6-164">Get-AzureRmSqlServerRecommendedActions</span><span class="sxs-lookup"><span data-stu-id="3c7a6-164">Get-AzureRmSqlServerRecommendedActions</span></span>
    + <span data-ttu-id="3c7a6-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="3c7a6-165">Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="3c7a6-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="3c7a6-166">Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="3c7a6-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span><span class="sxs-lookup"><span data-stu-id="3c7a6-167">Set-AzureRmSqlServerAdvisorAutoExecuteStatus</span></span>
    + <span data-ttu-id="3c7a6-168">Set-AzureRmSqlDatabaseRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="3c7a6-168">Set-AzureRmSqlDatabaseRecommendedActionState</span></span>
    + <span data-ttu-id="3c7a6-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="3c7a6-169">Set-AzureRmSqlElasticPoolRecommendedActionState</span></span>
    + <span data-ttu-id="3c7a6-170">Set-AzureRmSqlServerRecommendedActionState</span><span class="sxs-lookup"><span data-stu-id="3c7a6-170">Set-AzureRmSqlServerRecommendedActionState</span></span>
