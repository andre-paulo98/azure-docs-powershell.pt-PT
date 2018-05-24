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
# <a name="release-notes"></a>Notas de versão

Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.

## <a name="version-220"></a>Versão 2.2.0
* Computação
  - Adição de suporte para consultar o estado de encriptação a partir da extensão AzureDiskEncryptionForLinux
* DataFactory
  - Novo cmdlet adicionado para a listagem de janelas de atividade
    + Get-AzureRmDataFactoryActivityWindow
* DataLake
  - O parâmetro `Host` foi alterado para `DatabaseHost` e foi adicionado um alias a `Host`
    + New-AzureRmDataLakeAnalyticsCatalogSecret
    + Set-AzureRmDataLakeAnalyticsCatalogSecret
  - Adição de suporte para a remoção de ACL e ACL Predefinida
  - Adição de suporte para obter e definir permissões sem nome em ficheiros e pastas
* KeyVault
  - Adição de suporte para certificados
    + Add-AzureKeyVaultCertificate
    + Add-AzureKeyVaultCertificateContact
    + Get-AzureKeyVaultCertificate
    + Get-AzureKeyVaultCertificateContact
    + Get-AzureKeyVaultCertificateIssuer
    + Get-AzureKeyVaultCertificateOperation
    + Get-AzureKeyVaultCertificatePolicy
    + Import-AzureKeyVaultCertificate
    + New-AzureKeyVaultCertificateAdministratorDetails
    + New-AzureKeyVaultCertificateOrganizationDetails
    + New-AzureKeyVaultCertificatePolicy
    + Remove-AzureKeyVaultCertificate
    + Remove-AzureKeyVaultCertificateContact
    + Remove-AzureKeyVaultCertificateIssuer
    + Remove-AzureKeyVaultCertificateOperation
    + Set-AzureKeyVaultCertificateAttribute
    + Set-AzureKeyVaultCertificateIssuer
    + Set-AzureKeyVaultCertificatePolicy
    + Stop-AzureKeyVaultCertificateOperation
* Rede

  - Novo parâmetro opcional adicionado para a interface de rede ativar/desativar o funcionamento em rede acelerado +New-AzureRmNetworkInterface -EnableAcceleratedNetworking
  - Ativação de cmdlets do PowerShell da funcionalidade de gateway Ativo-Ativo
    + Add-AzureRmVirtualNetworkGatewayIpConfig
    + Remove-AzureRmVirtualNetworkGatewayIpConfig
  - Novo cmdlet adicionado
    + Test-AzureRmPrivateIpAddressAvailability
* Recursos
  - Zonas de suporte nos cmdlets de fornecedor e de recursos
    + Get-AzureRmProvider
    + New-AzureRmResource
    + Set-AzureRmResource
* SQL
  - Foram adicionados novos cmdlets para a gestão da política de deteção de ameaças de SQL do Azure ao nível do servidor
    + Get-AzureRmSqlServerThreatDetectionPolicy
    + Remove-AzureRmSqlServerThreatDetectionPolicy
    + Set-AzureRmSqlServerThreatDetectionPolicy
  - Foram adicionados novos cmdlets para suportar a ativação/desativação de GeoBackupPolicy para DataWarehouses do SQL Azure
    + Get-AzureRmSqlDatabaseGeoBackupPolicy
    + Set-AzureRmSqlDatabaseGeoBackupPolicy
  - Foram adicionados novos cmdlets para as APIs Ações Recomendadas e Assistentes de SQL
    + Get-AzureRmSqlDatabaseAdvisor
    + Get-AzureRmSqlElasticPoolAdvisor
    + Get-AzureRmSqlServerAdvisor
    + Get-AzureRmSqlDatabaseRecommendedActions
    + Get-AzureRmSqlElasticPoolRecommendedActions
    + Get-AzureRmSqlServerRecommendedActions
    + Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus
    + Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus
    + Set-AzureRmSqlServerAdvisorAutoExecuteStatus
    + Set-AzureRmSqlDatabaseRecommendedActionState
    + Set-AzureRmSqlElasticPoolRecommendedActionState
    + Set-AzureRmSqlServerRecommendedActionState
