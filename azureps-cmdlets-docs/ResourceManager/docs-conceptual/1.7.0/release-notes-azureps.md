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
ms.openlocfilehash: 0a3f152751fee569d3ac5fba6bcff8c1737f7b8c
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2017
---
# <a name="release-notes"></a><span data-ttu-id="c35d9-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="c35d9-103">Release notes</span></span>

<span data-ttu-id="c35d9-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="c35d9-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-170"></a><span data-ttu-id="c35d9-105">Versão 1.7.0</span><span class="sxs-lookup"><span data-stu-id="c35d9-105">Version 1.7.0</span></span>

* <span data-ttu-id="c35d9-106">**Alteração comportamental para os parâmetros -Force, –Confirm e $ConfirmPreference para todos os cmdlets. Estamos a alterar esta implementação para estar em conformidade com as diretrizes do PowerShell. Para a maioria dos cmdlets, isto significa remover o parâmetro Force e ignorar o pedido ShouldProcess; os utilizadores terão de incluir o parâmetro "-Confirm:$false" nos respetivos scripts do PowerShell.**</span><span class="sxs-lookup"><span data-stu-id="c35d9-106">**Behavioral change for -Force, –Confirm and $ConfirmPreference parameters for all cmdlets. We are changing this implementation to be in line with PowerShell guidelines. For most cmdlets, this means removing the Force parameter and to skip the ShouldProcess prompt, users will need to include the parameter: ‘-Confirm:$false’ in their PowerShell scripts.**</span></span> <span data-ttu-id="c35d9-107">Estas alterações visam os problemas seguintes:</span><span class="sxs-lookup"><span data-stu-id="c35d9-107">This changes are addressing following issues:</span></span>
  - <span data-ttu-id="c35d9-108">Implementação correta da funcionalidade –WhatIf, que permite que um utilizador determine os efeitos de um cmdlet ou script sem fazer alterações reais</span><span class="sxs-lookup"><span data-stu-id="c35d9-108">Correct implementation of –WhatIf functionality, allowing a user to determine the effects of a cmdlet or script without making any actual changes</span></span>
  - <span data-ttu-id="c35d9-109">Controlo sobre pedidos utilizando uma $ConfirmPreference em toda a sessão, de modo a que o utilizador seja avisado com base no impacto de uma alteração potencial (tal como relatado na definição ConfirmImpact no cmdlet)</span><span class="sxs-lookup"><span data-stu-id="c35d9-109">Control over prompting using a session-wide $ConfirmPreference, so that the user is prompted based on the impact of a prospective change (as reported in the ConfirmImpact setting in the cmdlet)</span></span>
  - <span data-ttu-id="c35d9-110">Controlo específico do cmdlet sobre pedidos de confirmação utilizando o parâmetro –Confirm</span><span class="sxs-lookup"><span data-stu-id="c35d9-110">Cmdlet-specific control over confirmation prompts using the –Confirm parameter</span></span>
  - <span data-ttu-id="c35d9-111">Utilização consistente de ShouldContinue e do parâmetro –Force em todos os cmdlets, para apenas as ações que precisem da confirmação do utilizador devido à natureza especial das alterações (por exemplo, eliminar ficheiros ocultos)</span><span class="sxs-lookup"><span data-stu-id="c35d9-111">Consistent use of ShouldContinue and the –Force parameter across cmdlets, for only those actions that would require prompting from the user due to the special nature of the changes (for example, deleting hidden files)</span></span>
  - <span data-ttu-id="c35d9-112">Consistência com outros cmdlets do PowerShell, para que o conhecimento de scripting do PowerShell de outros cmdlets seja imediatamente aplicável aos cmdlets do Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c35d9-112">Consistency with other PowerShell cmdlets, so that PowerShell scripting knowledge from other cmdlets is immediately applicable to the Azure PowerShell cmdlets.</span></span>

<span data-ttu-id="c35d9-113">**Tenha em atenção que agora, para *ignorar automaticamente todos os Pedidos em todas as Circunstâncias*, os cmdlets do Azure PowerShell exigem que o utilizador forneça dois parâmetros:**</span><span class="sxs-lookup"><span data-stu-id="c35d9-113">**Notice that now to *automatically skip all Prompts in all Circumstances* Azure PowerShell cmdlets require the user to supply two parameters:**</span></span>
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* <span data-ttu-id="c35d9-114">Computação do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-114">Azure Compute</span></span>
  - <span data-ttu-id="c35d9-115">Set-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="c35d9-115">Set-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="c35d9-116">Get-AzureRmVMADDomainExtension</span><span class="sxs-lookup"><span data-stu-id="c35d9-116">Get-AzureRmVMADDomainExtension</span></span>
  - <span data-ttu-id="c35d9-117">Parâmetro -Redeploy para Restart-AzureVM</span><span class="sxs-lookup"><span data-stu-id="c35d9-117">-Redeploy parameter for Restart-AzureVM</span></span>
  - <span data-ttu-id="c35d9-118">Parâmetro -Validate para Move-AzureService, Move-AzureStorageAccount e Move-AzureVirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="c35d9-118">-Validate parameter for Move-AzureService, Move-AzureStorageAccount, and Move-AzureVirtualNetwork</span></span>
  - <span data-ttu-id="c35d9-119">Os parâmetros de nome e versão para cmdlets de extensão são opcionais como antes.</span><span class="sxs-lookup"><span data-stu-id="c35d9-119">Name and version parameters for extension cmdlets are optional as before.</span></span>
  - <span data-ttu-id="c35d9-120">New-AzureVM pode obter um tipo de licença a partir do objeto VM.</span><span class="sxs-lookup"><span data-stu-id="c35d9-120">New-AzureVM can get a license type from VM object.</span></span>
* <span data-ttu-id="c35d9-121">Storage do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-121">Azure Storage</span></span>
  - <span data-ttu-id="c35d9-122">Alteração do Parâmetro de Etiquetas para Etiqueta e adição do alias do parâmetro Etiquetas</span><span class="sxs-lookup"><span data-stu-id="c35d9-122">Change Tags Parameter to Tag, and add parameter alias Tags</span></span>
    + <span data-ttu-id="c35d9-123">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-123">New-AzureRmStorageAccount</span></span>
    + <span data-ttu-id="c35d9-124">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-124">Set-AzureRmStorageAccount</span></span>
* <span data-ttu-id="c35d9-125">Rede do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-125">Azure Network</span></span>
  - <span data-ttu-id="c35d9-126">Novo cmdlet adicionado para Peering de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="c35d9-126">New cmdlet added for Virtual Network Peering</span></span>
* <span data-ttu-id="c35d9-127">Cache de Redis do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-127">Azure Redis Cache</span></span>
  - <span data-ttu-id="c35d9-128">Novo cmdlet adicionado para Reset-AzureRmRedisCache</span><span class="sxs-lookup"><span data-stu-id="c35d9-128">New cmdlet added for Reset-AzureRmRedisCache</span></span>
  - <span data-ttu-id="c35d9-129">Novo cmdlet adicionado para Export-AzureRmRedisCache</span><span class="sxs-lookup"><span data-stu-id="c35d9-129">New cmdlet added for Export-AzureRmRedisCache</span></span>
  - <span data-ttu-id="c35d9-130">Novo cmdlet adicionado para Import-AzureRmRedisCache</span><span class="sxs-lookup"><span data-stu-id="c35d9-130">New cmdlet added for Import-AzureRmRedisCache</span></span>
  - <span data-ttu-id="c35d9-131">O cmdlet New-AzureRmRedisCache foi modificado para incluir a alteração do parâmetro para vNet</span><span class="sxs-lookup"><span data-stu-id="c35d9-131">Modified cmdlet New-AzureRmRedisCache to include parameter change for vNet</span></span>
* <span data-ttu-id="c35d9-132">Cópia de Segurança/Restauro da BD SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-132">Azure SQL DB Backup/Restore</span></span>
  - <span data-ttu-id="c35d9-133">Cmdlets para a funcionalidade de cópia de segurança LTR (Retenção de Longo Prazo)</span><span class="sxs-lookup"><span data-stu-id="c35d9-133">Cmdlets for LTR (Long Term Retention) backup feature</span></span>
  - <span data-ttu-id="c35d9-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="c35d9-134">Get-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="c35d9-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c35d9-135">Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="c35d9-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span><span class="sxs-lookup"><span data-stu-id="c35d9-136">Set-AzureRmSqlServerBackupLongTermRetentionVault</span></span>
  - <span data-ttu-id="c35d9-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c35d9-137">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy</span></span>
  - <span data-ttu-id="c35d9-138">Restore-AzureRmSqlDatabase suporta agora o restauro para um ponto anterior no tempo de uma base de dados eliminada</span><span class="sxs-lookup"><span data-stu-id="c35d9-138">Restore-AzureRmSqlDatabase now supports point-in-time restore of a deleted database</span></span>
  - <span data-ttu-id="c35d9-139">Restore-AzureRmSqlDatabase suporta agora o restauro a partir de uma cópia de segurança de Retenção de Longo Prazo</span><span class="sxs-lookup"><span data-stu-id="c35d9-139">Restore-AzureRmSqlDatabase now supports restoring from a Long Term Retention backup</span></span>
* <span data-ttu-id="c35d9-140">Azure LogicApp</span><span class="sxs-lookup"><span data-stu-id="c35d9-140">Azure LogicApp</span></span>
  - <span data-ttu-id="c35d9-141">Foram adicionados cmdlets de contas de Integração de LogicApp.</span><span class="sxs-lookup"><span data-stu-id="c35d9-141">Added LogicApp Integration accounts cmdlets.</span></span>
  - <span data-ttu-id="c35d9-142">Get-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="c35d9-142">Get-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="c35d9-143">Get-AzureRmIntegrationAccountCallbackUrl</span><span class="sxs-lookup"><span data-stu-id="c35d9-143">Get-AzureRmIntegrationAccountCallbackUrl</span></span>
  - <span data-ttu-id="c35d9-144">Get-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="c35d9-144">Get-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="c35d9-145">Get-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-145">Get-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="c35d9-146">Get-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="c35d9-146">Get-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="c35d9-147">Get-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="c35d9-147">Get-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="c35d9-148">Get-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="c35d9-148">Get-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="c35d9-149">New-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="c35d9-149">New-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="c35d9-150">New-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="c35d9-150">New-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="c35d9-151">New-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-151">New-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="c35d9-152">New-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="c35d9-152">New-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="c35d9-153">New-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="c35d9-153">New-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="c35d9-154">New-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="c35d9-154">New-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="c35d9-155">Remove-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="c35d9-155">Remove-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="c35d9-156">Remove-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="c35d9-156">Remove-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="c35d9-157">Remove-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-157">Remove-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="c35d9-158">Remove-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="c35d9-158">Remove-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="c35d9-159">Remove-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="c35d9-159">Remove-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="c35d9-160">Remove-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="c35d9-160">Remove-AzureRmIntegrationAccountSchema</span></span>
  - <span data-ttu-id="c35d9-161">Set-AzureRmIntegrationAccountAgreement</span><span class="sxs-lookup"><span data-stu-id="c35d9-161">Set-AzureRmIntegrationAccountAgreement</span></span>
  - <span data-ttu-id="c35d9-162">Set-AzureRmIntegrationAccountCertificate</span><span class="sxs-lookup"><span data-stu-id="c35d9-162">Set-AzureRmIntegrationAccountCertificate</span></span>
  - <span data-ttu-id="c35d9-163">Set-AzureRmIntegrationAccount</span><span class="sxs-lookup"><span data-stu-id="c35d9-163">Set-AzureRmIntegrationAccount</span></span>
  - <span data-ttu-id="c35d9-164">Set-AzureRmIntegrationAccountMap</span><span class="sxs-lookup"><span data-stu-id="c35d9-164">Set-AzureRmIntegrationAccountMap</span></span>
  - <span data-ttu-id="c35d9-165">Set-AzureRmIntegrationAccountPartner</span><span class="sxs-lookup"><span data-stu-id="c35d9-165">Set-AzureRmIntegrationAccountPartner</span></span>
  - <span data-ttu-id="c35d9-166">Set-AzureRmIntegrationAccountSchema</span><span class="sxs-lookup"><span data-stu-id="c35d9-166">Set-AzureRmIntegrationAccountSchema</span></span>
* <span data-ttu-id="c35d9-167">Azure Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c35d9-167">Azure Data Lake Store</span></span>
  - <span data-ttu-id="c35d9-168">Melhoramento significativo do desempenho do carregamento e da transferência de ficheiros e pastas.</span><span class="sxs-lookup"><span data-stu-id="c35d9-168">Drastically improve performance of file and folder upload and download.</span></span>
  - <span data-ttu-id="c35d9-169">Isto inclui uma ligeira alteração aos nomes dos parâmetros para transferência e a inclusão de dois novos parâmetros para carregamento:</span><span class="sxs-lookup"><span data-stu-id="c35d9-169">This includes a slight change to the parameter names for download and inclusion of two new parameters for upload:</span></span>
    + <span data-ttu-id="c35d9-170">NumThreads -> PerFileThreadCount, utilizado para indicar o número de threads a utilizar num ficheiro único</span><span class="sxs-lookup"><span data-stu-id="c35d9-170">NumThreads -> PerFileThreadCount, used to indicate the number of threads to use in a single file</span></span>
    + <span data-ttu-id="c35d9-171">ConcurrentFileCount, utilizado para indicar o número de ficheiros a carregar/transferir em paralelo para o carregamento/transferência de pastas.</span><span class="sxs-lookup"><span data-stu-id="c35d9-171">ConcurrentFileCount, used to indicate the number of files to upload/download in parallel for folder upload/download.</span></span>
  - <span data-ttu-id="c35d9-172">Os valores de threading predefinidos visam agora proporcionar um melhor débito geral para a maioria dos tamanhos de ficheiro.</span><span class="sxs-lookup"><span data-stu-id="c35d9-172">Default threading values are now designed to give a better all around throughput for most file sizes.</span></span> <span data-ttu-id="c35d9-173">Se o desempenho não for o pretendido, os valores acima podem ser modificados para satisfazer os requisitos.</span><span class="sxs-lookup"><span data-stu-id="c35d9-173">If performance is not as desired, the values above can be modified to meet requirements.</span></span>
* <span data-ttu-id="c35d9-174">Azure Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c35d9-174">Azure Data Lake Analytics</span></span>
  - <span data-ttu-id="c35d9-175">Get-AzureRMDataLakeAnalyticsDataSource devolve agora todas as origens de dados quando é invocado sem argumentos.</span><span class="sxs-lookup"><span data-stu-id="c35d9-175">Get-AzureRMDataLakeAnalyticsDataSource now returns all data sources when called with no arguments.</span></span>
  - <span data-ttu-id="c35d9-176">Esta alteração também remove o parâmetro de tipo de origem de dados do cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c35d9-176">This change also removes the data source type parameter from the cmdlet.</span></span>
  - <span data-ttu-id="c35d9-177">Esta alteração resulta na devolução de um novo objeto para a operação de lista com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c35d9-177">This change results in a new object being returned for the list operation with the following properties:</span></span>
    + <span data-ttu-id="c35d9-178">Type, o tipo de origem de dados</span><span class="sxs-lookup"><span data-stu-id="c35d9-178">Type, the type of data source</span></span>
    + <span data-ttu-id="c35d9-179">Name, o nome da origem de dados</span><span class="sxs-lookup"><span data-stu-id="c35d9-179">Name, the name of the data source</span></span>
    + <span data-ttu-id="c35d9-180">IsDefault, definido como true se for a origem de dados predefinida para a conta</span><span class="sxs-lookup"><span data-stu-id="c35d9-180">IsDefault, set to true if this is the default data source for the account</span></span>
  - <span data-ttu-id="c35d9-181">Get-AzureRMDataLakeAnalyticsJob corrigido para lista para determinados valores de desvio de data e hora ao filtrar em submittedBefore e submittedAfter.</span><span class="sxs-lookup"><span data-stu-id="c35d9-181">Get-AzureRMDataLakeAnalyticsJob fixed for list for certain date time offset values when filtering on submittedBefore and submittedAfter.</span></span>
* <span data-ttu-id="c35d9-182">Aplicações Web</span><span class="sxs-lookup"><span data-stu-id="c35d9-182">Web Apps</span></span>
  - <span data-ttu-id="c35d9-183">Adição do cmdlet Swap-AzureRmWebAppSlot para troca regular e troca com pré-visualização</span><span class="sxs-lookup"><span data-stu-id="c35d9-183">Add Swap-AzureRmWebAppSlot cmdlet for regular swap and swap with preview</span></span>
  - <span data-ttu-id="c35d9-184">Expansão do cmdlet Set-AzureRmWebAppSlot para suportar a troca automática</span><span class="sxs-lookup"><span data-stu-id="c35d9-184">Extend Set-AzureRmWebAppSlot cmdlet to support auto swap</span></span>
* <span data-ttu-id="c35d9-185">API Management do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-185">Azure API Management</span></span>
  - <span data-ttu-id="c35d9-186">Correção dos cmdlets de Implementação de Gestão de API do Azure para AzureChinaCloud.</span><span class="sxs-lookup"><span data-stu-id="c35d9-186">Fixed Azure Api Management Deployment cmdlets for AzureChinaCloud.</span></span>
  - <span data-ttu-id="c35d9-187">Remoção do cmdlet Set-AzureRmApiManagementTenantGitAccess, uma vez que o Acesso Git está ativado por Predefinição.</span><span class="sxs-lookup"><span data-stu-id="c35d9-187">Removed cmdlet Set-AzureRmApiManagementTenantGitAccess as Git Access is enabled by Default.</span></span>
* <span data-ttu-id="c35d9-188">Cópia de Segurança dos Serviços de Recuperação do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-188">Azure Recovery Services Backup</span></span>
  - <span data-ttu-id="c35d9-189">Foi adicionado suporte para a carga de trabalho de SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-189">Added support for the Azure SQL workload</span></span>
  - <span data-ttu-id="c35d9-190">Foi adicionado suporte para a criação de cópias de segurança e restauro de VMs encriptadas do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-190">Added support for backing up and restoring encrypted Azure VMs</span></span>
  - <span data-ttu-id="c35d9-191">Backup-AzureRmRecoveryServicesBackupItem - Funcionalidade de período de retenção opcional adicionada para pontos de recuperação</span><span class="sxs-lookup"><span data-stu-id="c35d9-191">Backup-AzureRmRecoveryServicesBackupItem - Added optional retention time feature for recovery points</span></span>
  - <span data-ttu-id="c35d9-192">Pequenas correções de erros relacionados com filtros nos cmdlets Get-AzureRmRecoveryServicesBackupContainer e Get-AzureRmRecoveryServicesBackupItem</span><span class="sxs-lookup"><span data-stu-id="c35d9-192">Minor filter-related bug fixes in Get-AzureRmRecoveryServicesBackupContainer and Get-AzureRmRecoveryServicesBackupItem cmdlets</span></span>
* <span data-ttu-id="c35d9-193">Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="c35d9-193">Azure Automation</span></span>
  - <span data-ttu-id="c35d9-194">Get-AzureRmAutomationHybridWorkerGroup adicionado</span><span class="sxs-lookup"><span data-stu-id="c35d9-194">Added Get-AzureRmAutomationHybridWorkerGroup</span></span>
