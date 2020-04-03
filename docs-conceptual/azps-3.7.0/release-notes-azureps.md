---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 9e60e76206127922902804112e0b3f837cf03d76
ms.sourcegitcommit: eeb720e053939a68873ae3973bc81d5826358c9f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/31/2020
ms.locfileid: "80440508"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="0e245-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="0e245-103">Azure PowerShell release notes</span></span>
## <a name="370---march-2020"></a><span data-ttu-id="0e245-104">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="0e245-104">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-105">Az.Accounts</span></span>
* <span data-ttu-id="0e245-106">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="0e245-106">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-107">Az.Compute</span></span>
* <span data-ttu-id="0e245-108">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="0e245-108">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span> 
    - <span data-ttu-id="0e245-109">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="0e245-109">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="0e245-110">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="0e245-110">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="0e245-111">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="0e245-111">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="0e245-112">[#11354]</span><span class="sxs-lookup"><span data-stu-id="0e245-112">[#11354]</span></span>
* <span data-ttu-id="0e245-113">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="0e245-113">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="0e245-114">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="0e245-114">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="0e245-115">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="0e245-115">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="0e245-116">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="0e245-116">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="0e245-117">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="0e245-117">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="0e245-118">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-118">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="0e245-119">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="0e245-119">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="0e245-120">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="0e245-120">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="0e245-121">[#11257]</span><span class="sxs-lookup"><span data-stu-id="0e245-121">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-122">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-123">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="0e245-123">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="0e245-124">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="0e245-124">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-125">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-125">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-126">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="0e245-126">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="0e245-127">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="0e245-127">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-128">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-128">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-129">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="0e245-129">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-130">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-130">Az.IotHub</span></span>
* <span data-ttu-id="0e245-131">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e245-131">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="0e245-132">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-132">New Cmdlets are:</span></span>
    - <span data-ttu-id="0e245-133">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="0e245-133">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="0e245-134">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="0e245-134">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-135">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-135">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-136">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="0e245-136">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-137">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-137">Az.Monitor</span></span>
* <span data-ttu-id="0e245-138">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="0e245-138">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-139">Az.Network</span></span>
* <span data-ttu-id="0e245-140">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="0e245-140">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="0e245-141">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="0e245-141">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="0e245-142">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="0e245-142">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="0e245-143">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="0e245-143">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="0e245-144">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="0e245-144">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="0e245-145">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="0e245-145">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-146">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-146">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-147">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="0e245-147">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-148">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-148">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-149">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-149">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="0e245-150">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="0e245-150">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="0e245-151">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="0e245-151">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="0e245-152">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="0e245-152">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="0e245-153">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="0e245-153">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="0e245-154">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="0e245-154">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-155">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-155">Az.Resources</span></span>
* <span data-ttu-id="0e245-156">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="0e245-156">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="0e245-157">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="0e245-157">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="0e245-158">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="0e245-158">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="0e245-159">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="0e245-159">Added example.</span></span>
* <span data-ttu-id="0e245-160">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="0e245-160">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="0e245-161">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="0e245-161">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-162">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-162">Az.Sql</span></span>
* <span data-ttu-id="0e245-163">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="0e245-163">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="0e245-164">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="0e245-164">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="0e245-165">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="0e245-165">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="0e245-166">Az.Support</span><span class="sxs-lookup"><span data-stu-id="0e245-166">Az.Support</span></span>
* <span data-ttu-id="0e245-167">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="0e245-167">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-168">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-168">Az.Websites</span></span>
* <span data-ttu-id="0e245-169">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="0e245-169">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="0e245-170">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="0e245-170">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="0e245-171">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="0e245-171">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="0e245-172">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="0e245-172">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="0e245-173">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="0e245-173">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="0e245-174">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="0e245-174">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-175">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-175">Az.Accounts</span></span>
* <span data-ttu-id="0e245-176">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="0e245-176">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="0e245-177">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="0e245-177">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="0e245-178">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="0e245-178">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="0e245-179">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-179">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-180">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="0e245-180">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="0e245-181">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="0e245-181">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="0e245-182">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="0e245-182">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="0e245-183">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="0e245-183">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-184">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-184">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-185">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="0e245-185">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-186">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-186">Az.IotHub</span></span>
* <span data-ttu-id="0e245-187">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-187">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="0e245-188">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-188">New Cmdlets are:</span></span>
    - <span data-ttu-id="0e245-189">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-189">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-190">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-190">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-191">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-191">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-192">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-192">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="0e245-193">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-193">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="0e245-194">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-194">New Cmdlets are:</span></span>
    - <span data-ttu-id="0e245-195">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="0e245-195">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="0e245-196">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="0e245-196">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="0e245-197">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="0e245-197">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="0e245-198">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="0e245-198">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="0e245-199">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-199">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="0e245-200">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-200">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="0e245-201">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-201">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="0e245-202">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-202">New Cmdlets are:</span></span>
    - <span data-ttu-id="0e245-203">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="0e245-203">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="0e245-204">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="0e245-204">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="0e245-205">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e245-205">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-206">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-206">Az.Monitor</span></span>
* <span data-ttu-id="0e245-207">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="0e245-207">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-208">Az.Network</span></span>
* <span data-ttu-id="0e245-209">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="0e245-209">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="0e245-210">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="0e245-210">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="0e245-211">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="0e245-211">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="0e245-212">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="0e245-212">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-213">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-213">Az.Resources</span></span>
* <span data-ttu-id="0e245-214">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="0e245-214">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="0e245-215">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="0e245-215">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="0e245-216">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="0e245-216">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="0e245-217">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="0e245-217">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="0e245-218">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="0e245-218">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="0e245-219">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="0e245-219">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="0e245-220">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="0e245-220">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="0e245-221">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-221">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="0e245-222">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-222">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="0e245-223">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-223">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="0e245-224">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-224">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="0e245-225">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="0e245-225">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="0e245-226">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-226">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="0e245-227">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="0e245-227">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-228">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-228">Az.Sql</span></span>
* <span data-ttu-id="0e245-229">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="0e245-229">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="0e245-230">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="0e245-230">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="0e245-231">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="0e245-231">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="0e245-232">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="0e245-232">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="0e245-233">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="0e245-233">Remove an LTR backup</span></span>
    - <span data-ttu-id="0e245-234">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="0e245-234">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="0e245-235">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="0e245-235">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="0e245-236">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-236">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="0e245-237">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-237">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-238">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-238">Az.Storage</span></span>
* <span data-ttu-id="0e245-239">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-239">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="0e245-240">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="0e245-240">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="0e245-241">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="0e245-241">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="0e245-242">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="0e245-242">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="0e245-243">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="0e245-243">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-244">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-244">Az.Websites</span></span>
* <span data-ttu-id="0e245-245">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="0e245-245">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="0e245-246">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="0e245-246">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="0e245-247">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="0e245-247">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="0e245-248">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="0e245-248">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="0e245-249">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="0e245-249">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="0e245-250">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="0e245-250">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-251">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-251">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-252">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="0e245-252">Updated client side telemetry.</span></span>
* <span data-ttu-id="0e245-253">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0e245-253">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="0e245-254">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="0e245-254">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-255">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-255">Az.Accounts</span></span>
* <span data-ttu-id="0e245-256">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="0e245-256">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-257">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-257">Az.Automation</span></span>
* <span data-ttu-id="0e245-258">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="0e245-258">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-259">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-259">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-260">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="0e245-260">Updated SDK to 7.0</span></span>
* <span data-ttu-id="0e245-261">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="0e245-261">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-262">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-262">Az.Compute</span></span>
* <span data-ttu-id="0e245-263">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="0e245-263">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-264">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-264">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-265">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="0e245-265">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-266">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-266">Az.IotHub</span></span>
* <span data-ttu-id="0e245-267">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="0e245-267">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="0e245-268">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-268">New Cmdlets are:</span></span>
    - <span data-ttu-id="0e245-269">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-269">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-270">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-270">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-271">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-271">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="0e245-272">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="0e245-272">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-273">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-273">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-274">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="0e245-274">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-275">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-275">Az.Monitor</span></span>
* <span data-ttu-id="0e245-276">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="0e245-276">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="0e245-277">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="0e245-277">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="0e245-278">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="0e245-278">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-279">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-279">Az.Network</span></span>
* <span data-ttu-id="0e245-280">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="0e245-280">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="0e245-281">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="0e245-281">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="0e245-282">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="0e245-282">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="0e245-283">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="0e245-283">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="0e245-284">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0e245-284">No new cmdlets are added.</span></span> <span data-ttu-id="0e245-285">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="0e245-285">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-286">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-286">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-287">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="0e245-287">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-288">Az.Resources</span></span>
* <span data-ttu-id="0e245-289">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="0e245-289">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="0e245-290">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="0e245-290">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="0e245-291">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="0e245-291">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="0e245-292">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="0e245-292">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="0e245-293">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="0e245-293">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="0e245-294">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="0e245-294">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="0e245-295">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="0e245-295">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="0e245-296">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="0e245-296">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-297">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-297">Az.Sql</span></span>
* <span data-ttu-id="0e245-298">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="0e245-298">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="0e245-299">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="0e245-299">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="0e245-300">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="0e245-300">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="0e245-301">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="0e245-301">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="0e245-302">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="0e245-302">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="0e245-303">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="0e245-303">Az.StorageSync</span></span>
* <span data-ttu-id="0e245-304">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="0e245-304">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="0e245-305">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="0e245-305">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-306">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-306">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-307">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="0e245-307">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="0e245-308">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="0e245-308">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-309">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-309">Az.Accounts</span></span>
* <span data-ttu-id="0e245-310">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="0e245-310">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="0e245-311">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="0e245-311">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="0e245-312">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-312">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-313">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="0e245-313">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="0e245-314">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="0e245-314">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="0e245-315">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="0e245-315">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="0e245-316">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="0e245-316">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-317">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-317">Az.Compute</span></span>
* <span data-ttu-id="0e245-318">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="0e245-318">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="0e245-319">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="0e245-319">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="0e245-320">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-320">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="0e245-321">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-321">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="0e245-322">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="0e245-322">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-323">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-323">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-324">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="0e245-324">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="0e245-325">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="0e245-325">Az.DeploymentManager</span></span>
* <span data-ttu-id="0e245-326">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="0e245-326">Adds LIST operations for resources</span></span>
* <span data-ttu-id="0e245-327">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="0e245-327">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-328">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-328">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-329">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="0e245-329">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-330">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-330">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-331">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="0e245-331">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-332">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-332">Az.Network</span></span>
* <span data-ttu-id="0e245-333">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="0e245-333">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="0e245-334">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="0e245-334">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="0e245-335">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-335">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="0e245-336">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="0e245-336">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="0e245-337">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="0e245-337">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="0e245-338">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="0e245-338">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="0e245-339">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="0e245-339">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="0e245-340">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="0e245-340">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="0e245-341">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-341">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-342">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-342">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="0e245-343">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-343">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="0e245-344">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="0e245-344">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="0e245-345">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="0e245-345">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-346">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-346">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-347">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="0e245-347">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="0e245-348">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="0e245-348">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="0e245-349">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="0e245-349">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="0e245-350">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="0e245-350">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-351">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-351">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-352">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="0e245-352">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="0e245-353">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="0e245-353">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-354">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-354">Az.Resources</span></span>
* <span data-ttu-id="0e245-355">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="0e245-355">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="0e245-356">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="0e245-356">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-357">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-357">Az.Sql</span></span>
<span data-ttu-id="0e245-358">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="0e245-358">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-359">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-359">Az.Storage</span></span>
* <span data-ttu-id="0e245-360">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e245-360">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="0e245-361">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-361">New-AzStorageAccount</span></span>
* <span data-ttu-id="0e245-362">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="0e245-362">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="0e245-363">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-363">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-364">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-364">Az.Websites</span></span>
* <span data-ttu-id="0e245-365">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="0e245-365">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="0e245-366">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="0e245-366">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="0e245-367">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="0e245-367">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-368">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-368">Az.Accounts</span></span>
* <span data-ttu-id="0e245-369">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="0e245-369">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-370">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-370">Az.Cdn</span></span>
* <span data-ttu-id="0e245-371">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-371">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-372">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-372">Az.Compute</span></span>
* <span data-ttu-id="0e245-373">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="0e245-373">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="0e245-374">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-374">Az.ContainerInstance</span></span>
* <span data-ttu-id="0e245-375">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-375">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="0e245-376">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="0e245-376">Az.DataBoxEdge</span></span>
* <span data-ttu-id="0e245-377">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="0e245-377">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="0e245-378">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-378">Get the Edge Storage Container</span></span>
* <span data-ttu-id="0e245-379">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="0e245-379">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="0e245-380">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-380">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="0e245-381">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="0e245-381">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="0e245-382">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-382">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="0e245-383">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="0e245-383">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="0e245-384">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-384">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="0e245-385">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="0e245-385">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="0e245-386">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-386">Get the Edge Storage Account</span></span>
* <span data-ttu-id="0e245-387">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="0e245-387">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="0e245-388">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-388">Create new Edge Storage Account</span></span>
* <span data-ttu-id="0e245-389">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="0e245-389">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="0e245-390">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="0e245-390">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="0e245-391">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="0e245-391">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="0e245-392">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="0e245-392">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="0e245-393">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="0e245-393">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="0e245-394">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="0e245-394">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-395">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-395">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-396">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="0e245-396">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="0e245-397">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="0e245-397">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="0e245-398">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="0e245-398">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="0e245-399">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="0e245-399">Az.DevTestLabs</span></span>
* <span data-ttu-id="0e245-400">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="0e245-400">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-401">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-401">Az.EventHub</span></span>
* <span data-ttu-id="0e245-402">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="0e245-402">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-403">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-403">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-404">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="0e245-404">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="0e245-405">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="0e245-405">Az.MachineLearning</span></span>
* <span data-ttu-id="0e245-406">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="0e245-406">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="0e245-407">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="0e245-407">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="0e245-408">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="0e245-408">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="0e245-409">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="0e245-409">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="0e245-410">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="0e245-410">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="0e245-411">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="0e245-411">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="0e245-412">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="0e245-412">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="0e245-413">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="0e245-413">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-414">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-414">Az.Network</span></span>
* <span data-ttu-id="0e245-415">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="0e245-415">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-416">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-416">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-417">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-417">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="0e245-418">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-418">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="0e245-419">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-419">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="0e245-420">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-420">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-421">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-421">Az.Resources</span></span>
* <span data-ttu-id="0e245-422">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="0e245-422">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-423">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-423">Az.Sql</span></span>
* <span data-ttu-id="0e245-424">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="0e245-424">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="0e245-425">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="0e245-425">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="0e245-426">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="0e245-426">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="0e245-427">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="0e245-427">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-428">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-428">Az.Storage</span></span>
* <span data-ttu-id="0e245-429">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="0e245-429">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="0e245-430">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-430">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="0e245-431">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="0e245-431">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="0e245-432">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-432">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="0e245-433">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-433">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="0e245-434">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-434">General</span></span>
* <span data-ttu-id="0e245-435">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="0e245-435">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-436">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-436">Az.Accounts</span></span>
* <span data-ttu-id="0e245-437">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="0e245-437">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="0e245-438">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="0e245-438">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="0e245-439">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-439">Az.Batch</span></span>
* <span data-ttu-id="0e245-440">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="0e245-440">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-441">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-441">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-442">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="0e245-442">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-443">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-443">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-444">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="0e245-444">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="0e245-445">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="0e245-445">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="0e245-446">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="0e245-446">Az.HealthcareApis</span></span>
* <span data-ttu-id="0e245-447">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="0e245-447">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-448">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-448">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-449">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="0e245-449">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="0e245-450">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="0e245-450">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="0e245-451">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="0e245-451">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-452">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-452">Az.Monitor</span></span>
* <span data-ttu-id="0e245-453">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="0e245-453">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="0e245-454">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="0e245-454">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="0e245-455">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="0e245-455">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-456">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-456">Az.Network</span></span>
* <span data-ttu-id="0e245-457">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="0e245-457">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-458">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-458">Az.Resources</span></span>
* <span data-ttu-id="0e245-459">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="0e245-459">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="0e245-460">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="0e245-460">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-461">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-461">Az.Sql</span></span>
* <span data-ttu-id="0e245-462">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="0e245-462">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-463">Az.Storage</span></span>
* <span data-ttu-id="0e245-464">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="0e245-464">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="0e245-465">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="0e245-465">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="0e245-466">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="0e245-466">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="0e245-467">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="0e245-467">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="0e245-468">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="0e245-468">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="0e245-469">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="0e245-469">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="0e245-470">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="0e245-470">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="0e245-471">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-471">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="0e245-472">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-472">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="0e245-473">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="0e245-473">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="0e245-474">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="0e245-474">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="0e245-475">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="0e245-475">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="0e245-476">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="0e245-476">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="0e245-477">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-477">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-478">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-478">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-479">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="0e245-479">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="0e245-480">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="0e245-480">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-481">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-481">Az.Compute</span></span>
* <span data-ttu-id="0e245-482">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="0e245-482">VM Reapply feature</span></span>
    - <span data-ttu-id="0e245-483">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="0e245-483">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="0e245-484">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="0e245-484">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="0e245-485">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-485">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="0e245-486">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="0e245-486">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="0e245-487">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-487">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="0e245-488">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="0e245-488">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="0e245-489">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="0e245-489">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="0e245-490">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="0e245-490">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="0e245-491">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="0e245-491">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="0e245-492">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-492">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="0e245-493">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="0e245-493">Az.DataBoxEdge</span></span>
* <span data-ttu-id="0e245-494">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="0e245-494">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="0e245-495">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="0e245-495">Get the Order</span></span>
* <span data-ttu-id="0e245-496">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="0e245-496">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="0e245-497">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="0e245-497">Create new Order</span></span>
* <span data-ttu-id="0e245-498">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="0e245-498">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="0e245-499">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="0e245-499">Remove the Order</span></span>
* <span data-ttu-id="0e245-500">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="0e245-500">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="0e245-501">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="0e245-501">Now creates Local Share</span></span>
* <span data-ttu-id="0e245-502">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="0e245-502">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="0e245-503">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="0e245-503">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="0e245-504">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="0e245-504">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="0e245-505">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0e245-505">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="0e245-506">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="0e245-506">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="0e245-507">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="0e245-507">Gets the information about Triggers</span></span>
* <span data-ttu-id="0e245-508">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="0e245-508">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="0e245-509">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="0e245-509">Create new Triggers</span></span>
* <span data-ttu-id="0e245-510">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="0e245-510">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="0e245-511">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="0e245-511">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-512">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-512">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-513">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="0e245-513">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="0e245-514">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="0e245-514">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-515">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-515">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-516">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="0e245-516">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-517">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-517">Az.EventHub</span></span>
* <span data-ttu-id="0e245-518">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="0e245-518">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-519">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-519">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-520">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="0e245-520">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="0e245-521">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="0e245-521">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="0e245-522">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="0e245-522">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="0e245-523">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="0e245-523">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-524">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-524">Az.Network</span></span>
* <span data-ttu-id="0e245-525">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="0e245-525">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="0e245-526">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="0e245-526">Az.PrivateDns</span></span>
* <span data-ttu-id="0e245-527">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="0e245-527">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-528">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-528">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-529">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="0e245-529">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="0e245-530">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="0e245-530">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="0e245-531">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="0e245-531">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="0e245-532">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0e245-532">Az.RedisCache</span></span>
* <span data-ttu-id="0e245-533">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="0e245-533">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="0e245-534">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="0e245-534">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="0e245-535">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="0e245-535">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-536">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-536">Az.Resources</span></span>
- <span data-ttu-id="0e245-537">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="0e245-537">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="0e245-538">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="0e245-538">Updated create policy definition help example</span></span>
- <span data-ttu-id="0e245-539">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="0e245-539">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="0e245-540">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="0e245-540">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="0e245-541">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="0e245-541">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-542">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-542">Az.Sql</span></span>
* <span data-ttu-id="0e245-543">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="0e245-543">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="0e245-544">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="0e245-544">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="0e245-545">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-545">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="0e245-546">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-546">General</span></span>
* <span data-ttu-id="0e245-547">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="0e245-547">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-548">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-548">Az.Accounts</span></span>
* <span data-ttu-id="0e245-549">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="0e245-549">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="0e245-550">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="0e245-550">Az.Advisor</span></span>
* <span data-ttu-id="0e245-551">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="0e245-551">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="0e245-552">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-552">Az.Batch</span></span>
* <span data-ttu-id="0e245-553">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="0e245-553">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="0e245-554">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="0e245-554">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="0e245-555">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="0e245-555">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="0e245-556">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="0e245-556">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="0e245-557">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="0e245-557">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="0e245-558">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="0e245-558">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="0e245-559">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="0e245-559">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="0e245-560">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="0e245-560">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="0e245-561">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="0e245-561">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="0e245-562">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="0e245-562">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="0e245-563">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="0e245-563">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="0e245-564">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="0e245-564">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="0e245-565">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="0e245-565">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="0e245-566">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="0e245-566">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="0e245-567">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="0e245-567">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="0e245-568">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="0e245-568">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="0e245-569">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="0e245-569">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="0e245-570">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="0e245-570">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="0e245-571">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="0e245-571">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="0e245-572">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="0e245-572">This operation is no longer supported.</span></span>
* <span data-ttu-id="0e245-573">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="0e245-573">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="0e245-574">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="0e245-574">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="0e245-575">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="0e245-575">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="0e245-576">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="0e245-576">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="0e245-577">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="0e245-577">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="0e245-578">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="0e245-578">New non-verified images are also now returned.</span></span> <span data-ttu-id="0e245-579">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="0e245-579">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="0e245-580">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="0e245-580">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="0e245-581">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="0e245-581">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="0e245-582">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="0e245-582">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="0e245-583">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="0e245-583">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="0e245-584">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="0e245-584">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="0e245-585">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="0e245-585">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="0e245-586">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="0e245-586">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="0e245-587">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="0e245-587">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="0e245-588">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="0e245-588">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-589">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-589">Az.Cdn</span></span>
* <span data-ttu-id="0e245-590">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="0e245-590">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="0e245-591">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="0e245-591">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-592">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-592">Az.Compute</span></span>
* <span data-ttu-id="0e245-593">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="0e245-593">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="0e245-594">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="0e245-594">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="0e245-595">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="0e245-595">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="0e245-596">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-596">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="0e245-597">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-597">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="0e245-598">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="0e245-598">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="0e245-599">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-599">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="0e245-600">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="0e245-600">Breaking changes</span></span>
    - <span data-ttu-id="0e245-601">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="0e245-601">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="0e245-602">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="0e245-602">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-603">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-603">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-604">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="0e245-604">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-605">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-605">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-606">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="0e245-606">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="0e245-607">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="0e245-607">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="0e245-608">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="0e245-608">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="0e245-609">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="0e245-609">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="0e245-610">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="0e245-610">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="0e245-611">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="0e245-611">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-612">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-612">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-613">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="0e245-613">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-614">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-614">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-615">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="0e245-615">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="0e245-616">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="0e245-616">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="0e245-617">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="0e245-617">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="0e245-618">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-618">Removed five cmdlets:</span></span>
    - <span data-ttu-id="0e245-619">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="0e245-619">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="0e245-620">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="0e245-620">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="0e245-621">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="0e245-621">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="0e245-622">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="0e245-622">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="0e245-623">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="0e245-623">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="0e245-624">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-624">Added three cmdlets:</span></span>
    - <span data-ttu-id="0e245-625">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="0e245-625">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="0e245-626">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="0e245-626">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="0e245-627">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="0e245-627">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="0e245-628">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="0e245-628">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="0e245-629">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="0e245-629">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="0e245-630">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="0e245-630">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="0e245-631">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-631">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="0e245-632">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="0e245-632">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="0e245-633">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="0e245-633">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="0e245-634">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="0e245-634">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="0e245-635">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="0e245-635">Added some scenario test cases.</span></span>
* <span data-ttu-id="0e245-636">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="0e245-636">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-637">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-637">Az.IotHub</span></span>
* <span data-ttu-id="0e245-638">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="0e245-638">Breaking changes:</span></span>
    - <span data-ttu-id="0e245-639">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="0e245-639">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="0e245-640">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="0e245-640">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="0e245-641">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="0e245-641">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="0e245-642">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="0e245-642">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="0e245-643">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="0e245-643">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="0e245-644">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="0e245-644">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="0e245-645">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="0e245-645">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="0e245-646">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="0e245-646">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="0e245-647">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="0e245-647">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="0e245-648">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="0e245-648">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="0e245-649">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="0e245-649">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="0e245-650">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="0e245-650">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-651">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-651">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-652">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-652">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-653">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-653">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="0e245-654">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-654">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="0e245-655">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-655">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-656">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-656">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-657">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-657">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-658">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-658">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-659">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-659">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-660">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="0e245-660">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-661">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-661">Az.Resources</span></span>
* <span data-ttu-id="0e245-662">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="0e245-662">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-663">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-663">Az.Network</span></span>
* <span data-ttu-id="0e245-664">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="0e245-664">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="0e245-665">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-665">Updated cmdlet:</span></span>
        - <span data-ttu-id="0e245-666">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-666">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-667">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-667">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-668">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-668">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-669">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-669">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-670">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-670">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="0e245-671">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="0e245-671">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="0e245-672">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="0e245-672">New cmdlet:</span></span>
        - <span data-ttu-id="0e245-673">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="0e245-673">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="0e245-674">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="0e245-674">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="0e245-675">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-675">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="0e245-676">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-676">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="0e245-677">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="0e245-677">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="0e245-678">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="0e245-678">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="0e245-679">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-679">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="0e245-680">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="0e245-680">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="0e245-681">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-681">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-682">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="0e245-682">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="0e245-683">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-683">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="0e245-684">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-684">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="0e245-685">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-685">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="0e245-686">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="0e245-686">Set-AzVirtualHub</span></span>
* <span data-ttu-id="0e245-687">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="0e245-687">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="0e245-688">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="0e245-688">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="0e245-689">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="0e245-689">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="0e245-690">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="0e245-690">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="0e245-691">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="0e245-691">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="0e245-692">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="0e245-692">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="0e245-693">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-693">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="0e245-694">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-694">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-695">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-695">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="0e245-696">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="0e245-696">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="0e245-697">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="0e245-697">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="0e245-698">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="0e245-698">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="0e245-699">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="0e245-699">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="0e245-700">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="0e245-700">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="0e245-701">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="0e245-701">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="0e245-702">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="0e245-702">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="0e245-703">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-703">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-704">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="0e245-704">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="0e245-705">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="0e245-705">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="0e245-706">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="0e245-706">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="0e245-707">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="0e245-707">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="0e245-708">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="0e245-708">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="0e245-709">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-709">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="0e245-710">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="0e245-710">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="0e245-711">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="0e245-711">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="0e245-712">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="0e245-712">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="0e245-713">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="0e245-713">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="0e245-714">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="0e245-714">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="0e245-715">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="0e245-715">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="0e245-716">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="0e245-716">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="0e245-717">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="0e245-717">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="0e245-718">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="0e245-718">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="0e245-719">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="0e245-719">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="0e245-720">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-720">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="0e245-721">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-721">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-722">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-722">New-AzIpGroup</span></span>
        - <span data-ttu-id="0e245-723">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-723">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="0e245-724">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-724">Get-AzIpGroup</span></span>
        - <span data-ttu-id="0e245-725">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-725">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-726">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-726">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-727">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="0e245-727">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-728">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-728">Az.Sql</span></span>
* <span data-ttu-id="0e245-729">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="0e245-729">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="0e245-730">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="0e245-730">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="0e245-731">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="0e245-731">Removed deprecated aliases:</span></span>
* <span data-ttu-id="0e245-732">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="0e245-732">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="0e245-733">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="0e245-733">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="0e245-734">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-734">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="0e245-735">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="0e245-735">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="0e245-736">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="0e245-736">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="0e245-737">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="0e245-737">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-738">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-738">Az.Storage</span></span>
* <span data-ttu-id="0e245-739">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e245-739">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="0e245-740">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-740">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="0e245-741">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-741">Set-AzStorageAccount</span></span>
* <span data-ttu-id="0e245-742">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="0e245-742">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="0e245-743">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="0e245-743">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="0e245-744">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="0e245-744">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="0e245-745">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-745">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="0e245-746">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-746">General</span></span>
* <span data-ttu-id="0e245-747">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="0e245-747">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-748">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-748">Az.Accounts</span></span>
* <span data-ttu-id="0e245-749">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="0e245-749">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="0e245-750">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-750">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-751">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="0e245-751">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="0e245-752">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="0e245-752">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-753">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-753">Az.Automation</span></span>
* <span data-ttu-id="0e245-754">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="0e245-754">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="0e245-755">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-755">Az.Batch</span></span>
* <span data-ttu-id="0e245-756">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="0e245-756">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-757">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-757">Az.Compute</span></span>
* <span data-ttu-id="0e245-758">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-758">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="0e245-759">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="0e245-759">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="0e245-760">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="0e245-760">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="0e245-761">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="0e245-761">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-762">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-762">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-763">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="0e245-763">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="0e245-764">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="0e245-764">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="0e245-765">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="0e245-765">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-766">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-766">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-767">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="0e245-767">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="0e245-768">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="0e245-768">Az.HealthcareApis</span></span>
* <span data-ttu-id="0e245-769">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="0e245-769">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="0e245-770">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="0e245-770">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="0e245-771">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="0e245-771">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="0e245-772">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="0e245-772">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-773">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-773">Az.IotHub</span></span>
* <span data-ttu-id="0e245-774">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="0e245-774">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="0e245-775">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="0e245-775">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-776">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-776">Az.Monitor</span></span>
* <span data-ttu-id="0e245-777">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="0e245-777">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="0e245-778">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="0e245-778">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="0e245-779">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="0e245-779">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="0e245-780">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e245-780">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-781">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-781">Az.Network</span></span>
* <span data-ttu-id="0e245-782">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="0e245-782">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="0e245-783">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="0e245-783">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="0e245-784">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-784">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-785">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-785">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="0e245-786">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-786">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="0e245-787">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="0e245-787">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="0e245-788">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="0e245-788">Updated cmdlets:</span></span>
        - <span data-ttu-id="0e245-789">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-789">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="0e245-790">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-790">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="0e245-791">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-791">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="0e245-792">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="0e245-792">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="0e245-793">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="0e245-793">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="0e245-794">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="0e245-794">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="0e245-795">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="0e245-795">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="0e245-796">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0e245-796">Az.RedisCache</span></span>
* <span data-ttu-id="0e245-797">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="0e245-797">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-798">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-798">Az.Sql</span></span>
* <span data-ttu-id="0e245-799">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="0e245-799">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-800">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-800">Az.Storage</span></span>
* <span data-ttu-id="0e245-801">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="0e245-801">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="0e245-802">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="0e245-802">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="0e245-803">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="0e245-803">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="0e245-804">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="0e245-804">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="0e245-805">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-805">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="0e245-806">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="0e245-806">Az.StorageSync</span></span>
* <span data-ttu-id="0e245-807">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="0e245-807">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-808">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-808">Az.Websites</span></span>
* <span data-ttu-id="0e245-809">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="0e245-809">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="0e245-810">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-810">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="0e245-811">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-811">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-812">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="0e245-812">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="0e245-813">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="0e245-813">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="0e245-814">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="0e245-814">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-815">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-815">Az.Automation</span></span>
* <span data-ttu-id="0e245-816">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="0e245-816">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="0e245-817">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="0e245-817">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="0e245-818">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="0e245-818">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-819">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-819">Az.Compute</span></span>
* <span data-ttu-id="0e245-820">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-820">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="0e245-821">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-821">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="0e245-822">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="0e245-822">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="0e245-823">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="0e245-823">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="0e245-824">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="0e245-824">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="0e245-825">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="0e245-825">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="0e245-826">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="0e245-826">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="0e245-827">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="0e245-827">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="0e245-828">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="0e245-828">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-829">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-829">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-830">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="0e245-830">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="0e245-831">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="0e245-831">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-832">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-832">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-833">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="0e245-833">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-834">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-834">Az.IotHub</span></span>
* <span data-ttu-id="0e245-835">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="0e245-835">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="0e245-836">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="0e245-836">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="0e245-837">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="0e245-837">New cmdlets are:</span></span>
    - <span data-ttu-id="0e245-838">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="0e245-838">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="0e245-839">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="0e245-839">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="0e245-840">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="0e245-840">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="0e245-841">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="0e245-841">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-842">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-842">Az.Monitor</span></span>
* <span data-ttu-id="0e245-843">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="0e245-843">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="0e245-844">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="0e245-844">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="0e245-845">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0e245-845">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="0e245-846">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="0e245-846">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="0e245-847">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="0e245-847">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="0e245-848">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="0e245-848">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="0e245-849">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0e245-849">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="0e245-850">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="0e245-850">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="0e245-851">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="0e245-851">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="0e245-852">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="0e245-852">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="0e245-853">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="0e245-853">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="0e245-854">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="0e245-854">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="0e245-855">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="0e245-855">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="0e245-856">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="0e245-856">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="0e245-857">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="0e245-857">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="0e245-858">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="0e245-858">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="0e245-859">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="0e245-859">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="0e245-860">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-860">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="0e245-861">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="0e245-861">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="0e245-862">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-862">Overall improved help files</span></span>
* <span data-ttu-id="0e245-863">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="0e245-863">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-864">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-864">Az.Network</span></span>
* <span data-ttu-id="0e245-865">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="0e245-865">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="0e245-866">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="0e245-866">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="0e245-867">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="0e245-867">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="0e245-868">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="0e245-868">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="0e245-869">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="0e245-869">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="0e245-870">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="0e245-870">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="0e245-871">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="0e245-871">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="0e245-872">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="0e245-872">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="0e245-873">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-873">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="0e245-874">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="0e245-874">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="0e245-875">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="0e245-875">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="0e245-876">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="0e245-876">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="0e245-877">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-877">New cmdlets</span></span>
        - <span data-ttu-id="0e245-878">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="0e245-878">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="0e245-879">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-879">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="0e245-880">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-880">Updated cmdlet:</span></span>
        - <span data-ttu-id="0e245-881">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="0e245-881">New-VpnSite</span></span>
        - <span data-ttu-id="0e245-882">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="0e245-882">Update-VpnSite</span></span>
        - <span data-ttu-id="0e245-883">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-883">New-VpnConnection</span></span>
        - <span data-ttu-id="0e245-884">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-884">Update-VpnConnection</span></span>
* <span data-ttu-id="0e245-885">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="0e245-885">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-886">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-886">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-887">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="0e245-887">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="0e245-888">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="0e245-888">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-889">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-889">Az.Resources</span></span>
* <span data-ttu-id="0e245-890">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="0e245-890">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-891">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-891">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-892">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="0e245-892">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="0e245-893">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="0e245-893">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="0e245-894">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="0e245-894">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="0e245-895">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="0e245-895">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="0e245-896">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="0e245-896">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="0e245-897">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="0e245-897">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="0e245-898">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="0e245-898">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="0e245-899">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="0e245-899">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="0e245-900">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="0e245-900">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="0e245-901">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="0e245-901">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="0e245-902">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="0e245-902">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="0e245-903">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="0e245-903">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="0e245-904">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="0e245-904">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="0e245-905">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="0e245-905">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="0e245-906">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="0e245-906">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="0e245-907">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="0e245-907">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="0e245-908">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="0e245-908">Az.SignalR</span></span>
* <span data-ttu-id="0e245-909">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="0e245-909">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-910">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-910">Az.Sql</span></span>
* <span data-ttu-id="0e245-911">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="0e245-911">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="0e245-912">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="0e245-912">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="0e245-913">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-913">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="0e245-914">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="0e245-914">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="0e245-915">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="0e245-915">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-916">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-916">Az.Storage</span></span>
* <span data-ttu-id="0e245-917">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="0e245-917">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="0e245-918">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="0e245-918">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="0e245-919">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="0e245-919">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="0e245-920">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="0e245-920">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="0e245-921">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="0e245-921">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="0e245-922">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="0e245-922">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="0e245-923">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="0e245-923">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="0e245-924">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-924">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="0e245-925">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-925">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="0e245-926">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-926">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="0e245-927">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="0e245-927">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-928">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-928">Az.Websites</span></span>
* <span data-ttu-id="0e245-929">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="0e245-929">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="0e245-930">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="0e245-930">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="0e245-931">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="0e245-931">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="0e245-932">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-932">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="0e245-933">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-933">General</span></span>
* <span data-ttu-id="0e245-934">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="0e245-934">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-935">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-935">Az.Accounts</span></span>
* <span data-ttu-id="0e245-936">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="0e245-936">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="0e245-937">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="0e245-937">Az.Aks</span></span>
* <span data-ttu-id="0e245-938">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="0e245-938">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="0e245-939">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="0e245-939">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="0e245-940">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-940">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-941">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="0e245-941">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="0e245-942">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="0e245-942">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="0e245-943">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="0e245-943">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="0e245-944">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="0e245-944">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="0e245-945">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="0e245-945">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="0e245-946">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-946">Az.Batch</span></span>
* <span data-ttu-id="0e245-947">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="0e245-947">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-948">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-948">Az.Cdn</span></span>
* <span data-ttu-id="0e245-949">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="0e245-949">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-950">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-950">Az.Compute</span></span>
* <span data-ttu-id="0e245-951">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-951">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="0e245-952">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-952">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="0e245-953">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="0e245-953">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="0e245-954">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="0e245-954">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="0e245-955">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="0e245-955">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="0e245-956">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="0e245-956">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="0e245-957">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="0e245-957">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="0e245-958">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="0e245-958">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-959">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-959">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-960">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="0e245-960">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="0e245-961">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="0e245-961">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="0e245-962">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="0e245-962">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="0e245-963">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="0e245-963">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-964">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-964">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-965">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="0e245-965">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-966">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-966">Az.EventHub</span></span>
* <span data-ttu-id="0e245-967">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-967">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="0e245-968">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="0e245-968">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="0e245-969">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="0e245-969">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="0e245-970">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="0e245-970">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="0e245-971">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="0e245-971">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="0e245-972">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="0e245-972">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-973">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-973">Az.Monitor</span></span>
* <span data-ttu-id="0e245-974">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-974">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-975">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-975">Az.Network</span></span>
* <span data-ttu-id="0e245-976">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="0e245-976">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="0e245-977">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="0e245-977">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="0e245-978">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="0e245-978">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="0e245-979">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="0e245-979">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="0e245-980">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="0e245-980">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="0e245-981">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="0e245-981">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="0e245-982">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="0e245-982">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-983">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-983">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-984">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="0e245-984">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="0e245-985">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="0e245-985">Added example</span></span>
    - <span data-ttu-id="0e245-986">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="0e245-986">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="0e245-987">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="0e245-987">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="0e245-988">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="0e245-988">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-989">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-989">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-990">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-990">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-991">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-991">Az.Resources</span></span>
* <span data-ttu-id="0e245-992">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="0e245-992">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="0e245-993">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="0e245-993">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="0e245-994">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="0e245-994">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="0e245-995">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-995">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-996">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-996">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-997">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-997">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="0e245-998">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="0e245-998">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="0e245-999">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="0e245-999">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-1000">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1000">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-1001">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="0e245-1001">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="0e245-1002">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="0e245-1002">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="0e245-1003">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="0e245-1003">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="0e245-1004">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="0e245-1004">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="0e245-1005">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="0e245-1005">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="0e245-1006">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="0e245-1006">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1007">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1007">Az.Sql</span></span>
* <span data-ttu-id="0e245-1008">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="0e245-1008">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1009">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1009">Az.Storage</span></span>
* <span data-ttu-id="0e245-1010">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="0e245-1010">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="0e245-1011">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="0e245-1011">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="0e245-1012">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="0e245-1012">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="0e245-1013">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-1013">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="0e245-1014">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="0e245-1014">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="0e245-1015">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-1015">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1016">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1016">Az.Websites</span></span>
* <span data-ttu-id="0e245-1017">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="0e245-1017">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="0e245-1018">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1018">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1019">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1019">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1020">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="0e245-1020">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="0e245-1021">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1021">Az.ApplicationInsights</span></span>
* <span data-ttu-id="0e245-1022">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="0e245-1022">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1023">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1023">Az.Automation</span></span>
* <span data-ttu-id="0e245-1024">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="0e245-1024">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-1025">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1025">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-1026">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="0e245-1026">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1027">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1027">Az.Compute</span></span>
* <span data-ttu-id="0e245-1028">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="0e245-1028">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="0e245-1029">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="0e245-1029">Az.ContainerRegistry</span></span>
* <span data-ttu-id="0e245-1030">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="0e245-1030">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="0e245-1031">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="0e245-1031">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1032">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1032">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1033">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="0e245-1033">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="0e245-1034">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="0e245-1034">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-1035">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1035">Az.EventHub</span></span>
* <span data-ttu-id="0e245-1036">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="0e245-1036">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="0e245-1037">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="0e245-1037">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-1038">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1038">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-1039">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="0e245-1039">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="0e245-1040">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1040">Az.LogicApp</span></span>
* <span data-ttu-id="0e245-1041">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="0e245-1041">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="0e245-1042">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="0e245-1042">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="0e245-1043">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1043">Az.ManagedServices</span></span>
* <span data-ttu-id="0e245-1044">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="0e245-1044">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1045">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1045">Az.Network</span></span>
* <span data-ttu-id="0e245-1046">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="0e245-1046">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="0e245-1047">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1047">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1048">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-1048">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="0e245-1049">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1049">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="0e245-1050">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1050">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-1051">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1051">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-1052">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1052">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-1053">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1053">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="0e245-1054">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="0e245-1054">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="0e245-1055">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1055">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="0e245-1056">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="0e245-1056">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="0e245-1057">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1057">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="0e245-1058">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="0e245-1058">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="0e245-1059">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="0e245-1059">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="0e245-1060">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="0e245-1060">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="0e245-1061">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="0e245-1061">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="0e245-1062">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="0e245-1062">Updated cmdlets</span></span>
        - <span data-ttu-id="0e245-1063">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1063">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="0e245-1064">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1064">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="0e245-1065">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1065">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="0e245-1066">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1066">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="0e245-1067">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1067">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="0e245-1068">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-1068">Updated cmdlet:</span></span>
        - <span data-ttu-id="0e245-1069">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1069">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="0e245-1070">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1070">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="0e245-1071">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1071">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="0e245-1072">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="0e245-1072">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="0e245-1073">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="0e245-1073">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="0e245-1074">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="0e245-1074">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1075">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1075">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-1076">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="0e245-1076">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="0e245-1077">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="0e245-1077">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1078">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1078">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1079">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1079">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="0e245-1080">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1080">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="0e245-1081">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1081">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="0e245-1082">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1082">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="0e245-1083">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1083">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="0e245-1084">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1084">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="0e245-1085">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1085">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="0e245-1086">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1086">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="0e245-1087">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1087">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="0e245-1088">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="0e245-1088">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1089">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1089">Az.Resources</span></span>
- <span data-ttu-id="0e245-1090">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="0e245-1090">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="0e245-1091">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="0e245-1091">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-1092">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-1092">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-1093">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="0e245-1093">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="0e245-1094">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="0e245-1094">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1095">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1095">Az.Sql</span></span>
* <span data-ttu-id="0e245-1096">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="0e245-1096">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="0e245-1097">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="0e245-1097">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="0e245-1098">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="0e245-1098">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1099">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1099">Az.Storage</span></span>
* <span data-ttu-id="0e245-1100">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="0e245-1100">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="0e245-1101">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="0e245-1101">Az.StorageSync</span></span>
* <span data-ttu-id="0e245-1102">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="0e245-1102">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="0e245-1103">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="0e245-1103">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1104">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1104">Az.Websites</span></span>
* <span data-ttu-id="0e245-1105">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1105">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="0e245-1106">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1106">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="0e245-1107">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1107">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="0e245-1108">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1108">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1109">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1109">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1110">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="0e245-1110">Add support for profile cmdlets</span></span>
* <span data-ttu-id="0e245-1111">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="0e245-1111">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="0e245-1112">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="0e245-1112">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="0e245-1113">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="0e245-1113">Az.Advisor</span></span>
* <span data-ttu-id="0e245-1114">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="0e245-1114">GA release of Az.Advisor</span></span>
* <span data-ttu-id="0e245-1115">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="0e245-1115">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="0e245-1116">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-1116">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-1117">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="0e245-1117">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="0e245-1118">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="0e245-1118">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="0e245-1119">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="0e245-1119">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="0e245-1120">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="0e245-1120">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="0e245-1121">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="0e245-1121">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="0e245-1122">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="0e245-1122">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="0e245-1123">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="0e245-1123">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1124">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1124">Az.Automation</span></span>
* <span data-ttu-id="0e245-1125">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="0e245-1125">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1126">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1126">Az.Compute</span></span>
* <span data-ttu-id="0e245-1127">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1127">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1128">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1128">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1129">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="0e245-1129">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="0e245-1130">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0e245-1130">Az.EventGrid</span></span>
* <span data-ttu-id="0e245-1131">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="0e245-1131">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-1132">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1132">Az.IotHub</span></span>
* <span data-ttu-id="0e245-1133">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="0e245-1133">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1134">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1134">Az.Network</span></span>
* <span data-ttu-id="0e245-1135">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="0e245-1135">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="0e245-1136">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="0e245-1136">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-1137">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1137">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-1138">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="0e245-1138">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="0e245-1139">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="0e245-1139">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1140">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1140">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-1141">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="0e245-1141">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1142">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1143">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="0e245-1143">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1144">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1144">Az.Resources</span></span>
    - <span data-ttu-id="0e245-1145">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="0e245-1145">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="0e245-1146">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="0e245-1146">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="0e245-1147">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="0e245-1147">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="0e245-1148">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="0e245-1148">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-1149">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-1149">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-1150">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="0e245-1150">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1151">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1151">Az.Sql</span></span>
* <span data-ttu-id="0e245-1152">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="0e245-1152">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="0e245-1153">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1153">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="0e245-1154">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1154">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="0e245-1155">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1155">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="0e245-1156">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1156">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="0e245-1157">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1157">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="0e245-1158">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1158">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="0e245-1159">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="0e245-1159">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="0e245-1160">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="0e245-1160">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1161">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1161">Az.Storage</span></span>
* <span data-ttu-id="0e245-1162">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="0e245-1162">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="0e245-1163">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="0e245-1163">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="0e245-1164">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="0e245-1164">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="0e245-1165">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="0e245-1165">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="0e245-1166">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1166">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="0e245-1167">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1167">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="0e245-1168">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1168">Set-AzStorageAccount</span></span>
* <span data-ttu-id="0e245-1169">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="0e245-1169">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="0e245-1170">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="0e245-1170">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="0e245-1171">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="0e245-1171">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="0e245-1172">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="0e245-1172">Az.StorageSync</span></span>
* <span data-ttu-id="0e245-1173">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="0e245-1173">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="0e245-1174">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1174">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1175">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1175">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1176">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="0e245-1176">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="0e245-1177">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="0e245-1177">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="0e245-1178">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="0e245-1178">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="0e245-1179">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="0e245-1179">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="0e245-1180">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="0e245-1180">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1181">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1181">Az.Compute</span></span>
* <span data-ttu-id="0e245-1182">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="0e245-1182">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="0e245-1183">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="0e245-1183">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="0e245-1184">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="0e245-1184">Az.Dns</span></span>
* <span data-ttu-id="0e245-1185">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="0e245-1185">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="0e245-1186">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0e245-1186">Az.EventGrid</span></span>
* <span data-ttu-id="0e245-1187">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="0e245-1187">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="0e245-1188">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-1188">New cmdlets:</span></span>
    - <span data-ttu-id="0e245-1189">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="0e245-1189">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="0e245-1190">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="0e245-1190">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="0e245-1191">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="0e245-1191">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="0e245-1192">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-1192">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="0e245-1193">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="0e245-1193">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="0e245-1194">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="0e245-1194">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="0e245-1195">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="0e245-1195">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="0e245-1196">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="0e245-1196">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="0e245-1197">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="0e245-1197">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="0e245-1198">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="0e245-1198">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="0e245-1199">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="0e245-1199">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="0e245-1200">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="0e245-1200">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="0e245-1201">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="0e245-1201">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="0e245-1202">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="0e245-1202">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="0e245-1203">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="0e245-1203">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="0e245-1204">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="0e245-1204">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="0e245-1205">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="0e245-1205">Updated cmdlets:</span></span>
    - <span data-ttu-id="0e245-1206">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="0e245-1206">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="0e245-1207">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1207">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="0e245-1208">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1208">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="0e245-1209">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="0e245-1209">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="0e245-1210">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="0e245-1210">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="0e245-1211">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="0e245-1211">Event subscription expiration date,</span></span>
            - <span data-ttu-id="0e245-1212">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="0e245-1212">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="0e245-1213">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="0e245-1213">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="0e245-1214">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="0e245-1214">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="0e245-1215">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="0e245-1215">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="0e245-1216">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="0e245-1216">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="0e245-1217">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="0e245-1217">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="0e245-1218">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1218">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="0e245-1219">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1219">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-1220">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-1220">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-1221">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="0e245-1221">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="0e245-1222">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="0e245-1222">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="0e245-1223">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="0e245-1223">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="0e245-1224">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="0e245-1224">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1225">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1225">Az.Network</span></span>
* <span data-ttu-id="0e245-1226">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="0e245-1226">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="0e245-1227">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1227">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1228">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="0e245-1228">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="0e245-1229">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="0e245-1229">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="0e245-1230">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1230">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1231">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="0e245-1231">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="0e245-1232">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1232">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="0e245-1233">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1233">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1234">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1234">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="0e245-1235">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1235">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="0e245-1236">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="0e245-1236">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="0e245-1237">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1237">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="0e245-1238">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1238">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="0e245-1239">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-1239">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="0e245-1240">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1240">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1241">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-1241">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="0e245-1242">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-1242">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="0e245-1243">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="0e245-1243">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="0e245-1244">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1244">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="0e245-1245">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="0e245-1245">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="0e245-1246">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="0e245-1246">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="0e245-1247">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="0e245-1247">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="0e245-1248">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="0e245-1248">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="0e245-1249">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="0e245-1249">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="0e245-1250">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="0e245-1250">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="0e245-1251">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1251">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="0e245-1252">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="0e245-1252">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="0e245-1253">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1253">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="0e245-1254">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="0e245-1254">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="0e245-1255">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1255">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="0e245-1256">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1256">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="0e245-1257">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="0e245-1257">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="0e245-1258">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="0e245-1258">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="0e245-1259">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-1259">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="0e245-1260">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="0e245-1260">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="0e245-1261">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="0e245-1261">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="0e245-1262">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="0e245-1262">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="0e245-1263">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="0e245-1263">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="0e245-1264">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="0e245-1264">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="0e245-1265">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1265">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="0e245-1266">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1266">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="0e245-1267">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1267">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1268">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1268">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-1269">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="0e245-1269">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1270">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1270">Az.Resources</span></span>
* <span data-ttu-id="0e245-1271">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="0e245-1271">Support for additional Template Export options</span></span>
    - <span data-ttu-id="0e245-1272">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-1272">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="0e245-1273">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-1273">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="0e245-1274">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="0e245-1274">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-1275">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1275">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-1276">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="0e245-1276">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1277">Az.Sql</span></span>
* <span data-ttu-id="0e245-1278">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="0e245-1278">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="0e245-1279">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="0e245-1279">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="0e245-1280">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="0e245-1280">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="0e245-1281">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="0e245-1281">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="0e245-1282">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="0e245-1282">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="0e245-1283">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="0e245-1283">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="0e245-1284">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="0e245-1284">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="0e245-1285">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="0e245-1285">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1286">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1286">Az.Storage</span></span>
* <span data-ttu-id="0e245-1287">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e245-1287">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="0e245-1288">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1288">New-AzStorageAccount</span></span>
* <span data-ttu-id="0e245-1289">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="0e245-1289">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="0e245-1290">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1290">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1291">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1291">Az.Websites</span></span>
* <span data-ttu-id="0e245-1292">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="0e245-1292">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="0e245-1293">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="0e245-1293">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="0e245-1294">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1294">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="0e245-1295">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-1295">Az.Cdn</span></span>
* <span data-ttu-id="0e245-1296">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="0e245-1296">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1297">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1297">Az.Compute</span></span>
* <span data-ttu-id="0e245-1298">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="0e245-1298">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="0e245-1299">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="0e245-1299">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-1300">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1300">Az.EventHub</span></span>
* <span data-ttu-id="0e245-1301">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="0e245-1301">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="0e245-1302">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="0e245-1302">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1303">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1303">Az.Network</span></span>
* <span data-ttu-id="0e245-1304">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1304">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="0e245-1305">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="0e245-1305">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-1306">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1306">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-1307">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="0e245-1307">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1308">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1308">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1309">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="0e245-1309">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-1310">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-1310">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-1311">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="0e245-1311">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-1312">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1312">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-1313">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="0e245-1313">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="0e245-1314">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1314">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1315">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1315">Az.Sql</span></span>
* <span data-ttu-id="0e245-1316">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="0e245-1316">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="0e245-1317">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1317">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="0e245-1318">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="0e245-1318">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="0e245-1319">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="0e245-1319">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1320">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1320">Az.Websites</span></span>
* <span data-ttu-id="0e245-1321">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="0e245-1321">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="0e245-1322">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1322">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="0e245-1323">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-1323">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-1324">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="0e245-1324">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="0e245-1325">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="0e245-1325">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="0e245-1326">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="0e245-1326">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="0e245-1327">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="0e245-1327">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="0e245-1328">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1328">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="0e245-1329">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="0e245-1329">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="0e245-1330">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="0e245-1330">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="0e245-1331">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="0e245-1331">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="0e245-1332">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-1332">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="0e245-1333">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="0e245-1333">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="0e245-1334">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="0e245-1334">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="0e245-1335">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="0e245-1335">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="0e245-1336">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="0e245-1336">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="0e245-1337">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="0e245-1337">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="0e245-1338">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="0e245-1338">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="0e245-1339">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="0e245-1339">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="0e245-1340">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="0e245-1340">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="0e245-1341">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="0e245-1341">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="0e245-1342">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="0e245-1342">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="0e245-1343">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="0e245-1343">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="0e245-1344">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="0e245-1344">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="0e245-1345">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="0e245-1345">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="0e245-1346">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="0e245-1346">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="0e245-1347">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-1347">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="0e245-1348">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="0e245-1348">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="0e245-1349">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="0e245-1349">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="0e245-1350">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="0e245-1350">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="0e245-1351">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="0e245-1351">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="0e245-1352">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="0e245-1352">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="0e245-1353">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="0e245-1353">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="0e245-1354">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="0e245-1354">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="0e245-1355">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="0e245-1355">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="0e245-1356">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="0e245-1356">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="0e245-1357">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="0e245-1357">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="0e245-1358">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="0e245-1358">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="0e245-1359">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="0e245-1359">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="0e245-1360">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="0e245-1360">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="0e245-1361">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="0e245-1361">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="0e245-1362">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="0e245-1362">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="0e245-1363">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="0e245-1363">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="0e245-1364">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="0e245-1364">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="0e245-1365">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="0e245-1365">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="0e245-1366">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="0e245-1366">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="0e245-1367">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="0e245-1367">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="0e245-1368">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="0e245-1368">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="0e245-1369">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="0e245-1369">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="0e245-1370">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="0e245-1370">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="0e245-1371">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="0e245-1371">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="0e245-1372">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="0e245-1372">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="0e245-1373">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="0e245-1373">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="0e245-1374">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="0e245-1374">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="0e245-1375">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="0e245-1375">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="0e245-1376">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="0e245-1376">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="0e245-1377">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="0e245-1377">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="0e245-1378">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="0e245-1378">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="0e245-1379">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="0e245-1379">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="0e245-1380">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="0e245-1380">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="0e245-1381">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="0e245-1381">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="0e245-1382">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="0e245-1382">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="0e245-1383">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="0e245-1383">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="0e245-1384">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="0e245-1384">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="0e245-1385">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="0e245-1385">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="0e245-1386">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="0e245-1386">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="0e245-1387">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="0e245-1387">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="0e245-1388">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="0e245-1388">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="0e245-1389">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="0e245-1389">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="0e245-1390">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="0e245-1390">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="0e245-1391">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="0e245-1391">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="0e245-1392">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="0e245-1392">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="0e245-1393">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="0e245-1393">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="0e245-1394">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="0e245-1394">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="0e245-1395">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="0e245-1395">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="0e245-1396">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="0e245-1396">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="0e245-1397">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1397">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="0e245-1398">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="0e245-1398">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="0e245-1399">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="0e245-1399">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="0e245-1400">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="0e245-1400">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1401">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1401">Az.Automation</span></span>
* <span data-ttu-id="0e245-1402">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="0e245-1402">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="0e245-1403">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="0e245-1403">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="0e245-1404">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="0e245-1404">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="0e245-1405">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="0e245-1405">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="0e245-1406">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="0e245-1406">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="0e245-1407">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="0e245-1407">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="0e245-1408">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="0e245-1408">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1409">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1409">Az.Compute</span></span>
* <span data-ttu-id="0e245-1410">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="0e245-1410">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="0e245-1411">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="0e245-1411">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1412">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1412">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-1413">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1413">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-1414">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-1414">Az.Monitor</span></span>
* <span data-ttu-id="0e245-1415">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-1415">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1416">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1416">Az.Network</span></span>
* <span data-ttu-id="0e245-1417">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="0e245-1417">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="0e245-1418">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="0e245-1418">Updated cmdlet:</span></span>
        - <span data-ttu-id="0e245-1419">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-1419">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="0e245-1420">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0e245-1420">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1421">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1421">Az.Resources</span></span>
* <span data-ttu-id="0e245-1422">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="0e245-1422">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1423">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1423">Az.Sql</span></span>
* <span data-ttu-id="0e245-1424">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="0e245-1424">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="0e245-1425">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1425">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1426">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1426">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1427">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="0e245-1427">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-1428">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1428">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-1429">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="0e245-1429">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="0e245-1430">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="0e245-1430">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1431">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1431">Az.Compute</span></span>
* <span data-ttu-id="0e245-1432">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="0e245-1432">Proximity placement group feature.</span></span>
    - <span data-ttu-id="0e245-1433">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-1433">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="0e245-1434">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1434">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="0e245-1435">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="0e245-1435">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="0e245-1436">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="0e245-1436">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="0e245-1437">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-1437">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="0e245-1438">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="0e245-1438">Breaking changes</span></span>
    - <span data-ttu-id="0e245-1439">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="0e245-1439">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="0e245-1440">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="0e245-1440">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="0e245-1441">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="0e245-1441">Az.DeploymentManager</span></span>
* <span data-ttu-id="0e245-1442">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1442">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="0e245-1443">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="0e245-1443">Az.Dns</span></span>
* <span data-ttu-id="0e245-1444">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="0e245-1444">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="0e245-1445">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="0e245-1445">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="0e245-1446">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="0e245-1446">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="0e245-1447">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-1447">Az.FrontDoor</span></span>
* <span data-ttu-id="0e245-1448">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="0e245-1448">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="0e245-1449">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="0e245-1449">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="0e245-1450">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-1450">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-1451">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-1451">Removed two cmdlets:</span></span>
    - <span data-ttu-id="0e245-1452">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="0e245-1452">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="0e245-1453">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="0e245-1453">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="0e245-1454">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="0e245-1454">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="0e245-1455">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="0e245-1455">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="0e245-1456">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="0e245-1456">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="0e245-1457">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="0e245-1457">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-1458">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-1458">Az.Monitor</span></span>
* <span data-ttu-id="0e245-1459">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="0e245-1459">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="0e245-1460">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="0e245-1460">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="0e245-1461">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-1461">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="0e245-1462">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="0e245-1462">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="0e245-1463">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="0e245-1463">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="0e245-1464">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="0e245-1464">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="0e245-1465">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="0e245-1465">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="0e245-1466">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1466">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="0e245-1467">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1467">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="0e245-1468">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1468">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="0e245-1469">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1469">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="0e245-1470">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1470">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="0e245-1471">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="0e245-1471">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="0e245-1472">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="0e245-1472">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1473">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1473">Az.Network</span></span>
* <span data-ttu-id="0e245-1474">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="0e245-1474">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="0e245-1475">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1475">New cmdlets</span></span>
        - <span data-ttu-id="0e245-1476">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1476">New-AzNatGateway</span></span>
        - <span data-ttu-id="0e245-1477">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1477">Get-AzNatGateway</span></span>
        - <span data-ttu-id="0e245-1478">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1478">Set-AzNatGateway</span></span>
        - <span data-ttu-id="0e245-1479">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1479">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="0e245-1480">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="0e245-1480">Updated cmdlets</span></span>
        - <span data-ttu-id="0e245-1481">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="0e245-1481">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="0e245-1482">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="0e245-1482">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="0e245-1483">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1483">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="0e245-1484">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1484">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="0e245-1485">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="0e245-1485">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-1486">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1486">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-1487">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="0e245-1487">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="0e245-1488">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="0e245-1488">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="0e245-1489">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="0e245-1489">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1490">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1490">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1491">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="0e245-1491">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="0e245-1492">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="0e245-1492">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="0e245-1493">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="0e245-1493">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="0e245-1494">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-1494">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="0e245-1495">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1495">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="0e245-1496">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="0e245-1496">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="0e245-1497">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="0e245-1497">Az.Relay</span></span>
* <span data-ttu-id="0e245-1498">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="0e245-1498">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-1499">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-1499">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-1500">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="0e245-1500">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1501">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1501">Az.Storage</span></span>
* <span data-ttu-id="0e245-1502">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="0e245-1502">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="0e245-1503">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="0e245-1503">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="0e245-1504">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="0e245-1504">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="0e245-1505">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1505">New-AzStorageAccount</span></span>
* <span data-ttu-id="0e245-1506">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="0e245-1506">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="0e245-1507">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1507">New-AzStorageAccount</span></span>
    - <span data-ttu-id="0e245-1508">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1508">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="0e245-1509">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1509">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1510">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1510">Az.Websites</span></span>
* <span data-ttu-id="0e245-1511">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1511">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="0e245-1512">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="0e245-1512">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="0e245-1513">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1513">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-1514">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-1514">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-1515">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="0e245-1515">General availability of `Az` module</span></span>
* <span data-ttu-id="0e245-1516">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="0e245-1516">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="0e245-1517">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="0e245-1517">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="0e245-1518">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1518">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="0e245-1519">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="0e245-1519">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="0e245-1520">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1520">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="0e245-1521">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="0e245-1521">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-1522">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1522">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1523">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="0e245-1523">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="0e245-1524">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-1524">Az.Batch</span></span>
* <span data-ttu-id="0e245-1525">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1525">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-1526">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-1526">Az.Cdn</span></span>
* <span data-ttu-id="0e245-1527">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1527">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-1528">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1528">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-1529">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1529">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1530">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1530">Az.Compute</span></span>
* <span data-ttu-id="0e245-1531">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="0e245-1531">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="0e245-1532">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1532">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1533">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="0e245-1533">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1534">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1534">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1535">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="0e245-1535">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1536">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-1537">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1537">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="0e245-1538">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0e245-1538">Az.EventGrid</span></span>
* <span data-ttu-id="0e245-1539">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="0e245-1539">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-1540">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1540">Az.EventHub</span></span>
* <span data-ttu-id="0e245-1541">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="0e245-1541">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="0e245-1542">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="0e245-1542">Az.HDInsight</span></span>
* <span data-ttu-id="0e245-1543">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1543">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-1544">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1544">Az.IotHub</span></span>
* <span data-ttu-id="0e245-1545">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1545">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-1546">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1546">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-1547">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1547">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1548">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="0e245-1548">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="0e245-1549">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="0e245-1549">Az.MachineLearning</span></span>
* <span data-ttu-id="0e245-1550">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1550">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="0e245-1551">Az.Media</span><span class="sxs-lookup"><span data-stu-id="0e245-1551">Az.Media</span></span>
* <span data-ttu-id="0e245-1552">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1552">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-1553">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-1553">Az.Monitor</span></span>
  * <span data-ttu-id="0e245-1554">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="0e245-1554">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="0e245-1555">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="0e245-1555">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="0e245-1556">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="0e245-1556">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="0e245-1557">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="0e245-1557">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="0e245-1558">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="0e245-1558">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="0e245-1559">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="0e245-1559">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="0e245-1560">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="0e245-1560">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1561">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1561">Az.Network</span></span>
* <span data-ttu-id="0e245-1562">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1562">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1563">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="0e245-1563">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="0e245-1564">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="0e245-1564">Az.NotificationHubs</span></span>
* <span data-ttu-id="0e245-1565">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1565">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1566">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1566">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-1567">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1567">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="0e245-1568">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="0e245-1568">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="0e245-1569">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1569">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1570">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1570">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1571">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1571">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1572">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1572">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="0e245-1573">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="0e245-1573">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="0e245-1574">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="0e245-1574">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="0e245-1575">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0e245-1575">Az.RedisCache</span></span>
* <span data-ttu-id="0e245-1576">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1576">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1577">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1577">Az.Resources</span></span>
* <span data-ttu-id="0e245-1578">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="0e245-1578">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1579">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1579">Az.Sql</span></span>
* <span data-ttu-id="0e245-1580">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="0e245-1580">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="0e245-1581">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1581">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1582">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="0e245-1582">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="0e245-1583">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="0e245-1583">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="0e245-1584">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="0e245-1584">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="0e245-1585">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="0e245-1585">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="0e245-1586">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="0e245-1586">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1587">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1587">Az.Websites</span></span>
* <span data-ttu-id="0e245-1588">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="0e245-1588">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="0e245-1589">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="0e245-1589">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="0e245-1590">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="0e245-1590">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="0e245-1591">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="0e245-1591">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="0e245-1592">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1592">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-1593">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-1593">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-1594">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="0e245-1594">General availability of `Az` module</span></span>
* <span data-ttu-id="0e245-1595">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="0e245-1595">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="0e245-1596">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="0e245-1596">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="0e245-1597">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1597">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="0e245-1598">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="0e245-1598">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="0e245-1599">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1599">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="0e245-1600">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="0e245-1600">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="0e245-1601">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1601">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1602">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="0e245-1602">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="0e245-1603">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1603">Az.AnalysisServices</span></span>
* <span data-ttu-id="0e245-1604">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="0e245-1604">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="0e245-1605">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="0e245-1605">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1606">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1606">Az.Automation</span></span>
* <span data-ttu-id="0e245-1607">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="0e245-1607">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="0e245-1608">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="0e245-1608">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="0e245-1609">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1609">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1610">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1610">Az.Compute</span></span>
* <span data-ttu-id="0e245-1611">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1611">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="0e245-1612">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1612">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="0e245-1613">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-1613">Az.ContainerInstance</span></span>
* <span data-ttu-id="0e245-1614">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="0e245-1614">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1615">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1615">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1616">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="0e245-1616">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="0e245-1617">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0e245-1617">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1618">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1618">Az.Resources</span></span>
* <span data-ttu-id="0e245-1619">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="0e245-1619">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="0e245-1620">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="0e245-1620">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="0e245-1621">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="0e245-1621">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="0e245-1622">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="0e245-1622">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="0e245-1623">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="0e245-1623">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="0e245-1624">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="0e245-1624">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1625">Az.Sql</span></span>
* <span data-ttu-id="0e245-1626">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="0e245-1626">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1627">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1627">Az.Storage</span></span>
* <span data-ttu-id="0e245-1628">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1628">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="0e245-1629">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="0e245-1629">New-AzStorageContext</span></span>
* <span data-ttu-id="0e245-1630">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="0e245-1630">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="0e245-1631">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="0e245-1631">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="0e245-1632">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="0e245-1632">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="0e245-1633">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1633">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="0e245-1634">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1634">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="0e245-1635">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="0e245-1635">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="0e245-1636">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="0e245-1636">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="0e245-1637">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="0e245-1637">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="0e245-1638">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="0e245-1638">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="0e245-1639">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="0e245-1639">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="0e245-1640">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1640">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="0e245-1641">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="0e245-1641">Highlights since the last major release</span></span>
* <span data-ttu-id="0e245-1642">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="0e245-1642">General availability of `Az` module</span></span>
* <span data-ttu-id="0e245-1643">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="0e245-1643">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="0e245-1644">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="0e245-1644">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="0e245-1645">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1645">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="0e245-1646">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="0e245-1646">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="0e245-1647">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1647">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="0e245-1648">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="0e245-1648">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1649">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1649">Az.Automation</span></span>
* <span data-ttu-id="0e245-1650">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="0e245-1650">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="0e245-1651">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="0e245-1651">Dynamic grouping</span></span>
    * <span data-ttu-id="0e245-1652">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="0e245-1652">Pre-Post script</span></span>
    * <span data-ttu-id="0e245-1653">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="0e245-1653">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1654">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1654">Az.Compute</span></span>
* <span data-ttu-id="0e245-1655">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="0e245-1655">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="0e245-1656">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="0e245-1656">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-1657">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1657">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-1658">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1658">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1659">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1659">Az.Network</span></span>
* <span data-ttu-id="0e245-1660">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="0e245-1660">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="0e245-1661">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="0e245-1661">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1662">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1662">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1663">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="0e245-1663">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="0e245-1664">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="0e245-1664">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1665">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1665">Az.Resources</span></span>
* <span data-ttu-id="0e245-1666">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-1666">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="0e245-1667">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="0e245-1667">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1668">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1668">Az.Sql</span></span>
* <span data-ttu-id="0e245-1669">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="0e245-1669">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1670">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1670">Az.Storage</span></span>
* <span data-ttu-id="0e245-1671">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="0e245-1671">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="0e245-1672">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1672">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="0e245-1673">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1673">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="0e245-1674">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1674">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="0e245-1675">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="0e245-1675">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="0e245-1676">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="0e245-1676">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="0e245-1677">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1677">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1678">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1678">Az.Websites</span></span>
* <span data-ttu-id="0e245-1679">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="0e245-1679">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="0e245-1680">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1680">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1681">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1681">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1682">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="0e245-1682">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="0e245-1683">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1683">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1684">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1684">Az.Automation</span></span>
* <span data-ttu-id="0e245-1685">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1685">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="0e245-1686">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="0e245-1686">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="0e245-1687">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="0e245-1687">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-1688">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-1688">Az.Cdn</span></span>
* <span data-ttu-id="0e245-1689">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="0e245-1689">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1690">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1690">Az.Compute</span></span>
* <span data-ttu-id="0e245-1691">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="0e245-1691">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1692">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1692">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1693">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="0e245-1693">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="0e245-1694">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1694">Az.LogicApp</span></span>
* <span data-ttu-id="0e245-1695">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="0e245-1695">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1696">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1696">Az.Network</span></span>
* <span data-ttu-id="0e245-1697">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1697">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1698">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1698">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1699">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-1699">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="0e245-1700">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="0e245-1700">SDK Update</span></span>
* <span data-ttu-id="0e245-1701">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="0e245-1701">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="0e245-1702">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="0e245-1702">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1703">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1703">Az.Resources</span></span>
* <span data-ttu-id="0e245-1704">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="0e245-1704">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="0e245-1705">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="0e245-1705">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="0e245-1706">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="0e245-1706">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="0e245-1707">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="0e245-1707">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="0e245-1708">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="0e245-1708">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="0e245-1709">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="0e245-1709">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1710">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1710">Az.Sql</span></span>
* <span data-ttu-id="0e245-1711">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="0e245-1711">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="0e245-1712">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="0e245-1712">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1713">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1713">Az.Storage</span></span>
* <span data-ttu-id="0e245-1714">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1714">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="0e245-1715">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1715">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="0e245-1716">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1716">Az.AnalysisServices</span></span>
* <span data-ttu-id="0e245-1717">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="0e245-1717">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1718">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1718">Az.Automation</span></span>
* <span data-ttu-id="0e245-1719">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1719">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="0e245-1720">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1720">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="0e245-1721">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1721">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-1722">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1722">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-1723">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="0e245-1723">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1724">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1724">Az.Compute</span></span>
* <span data-ttu-id="0e245-1725">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="0e245-1725">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="0e245-1726">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="0e245-1726">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="0e245-1727">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="0e245-1727">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="0e245-1728">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="0e245-1728">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1729">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1729">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-1730">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="0e245-1730">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="0e245-1731">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1731">Az.EventHub</span></span>
* <span data-ttu-id="0e245-1732">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="0e245-1732">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-1733">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1733">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-1734">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="0e245-1734">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="0e245-1735">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1735">Az.LogicApp</span></span>
* <span data-ttu-id="0e245-1736">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="0e245-1736">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="0e245-1737">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="0e245-1737">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="0e245-1738">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="0e245-1738">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="0e245-1739">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="0e245-1739">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="0e245-1740">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="0e245-1740">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="0e245-1741">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="0e245-1741">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="0e245-1742">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="0e245-1742">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="0e245-1743">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="0e245-1743">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="0e245-1744">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1744">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="0e245-1745">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1745">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="0e245-1746">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1746">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="0e245-1747">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1747">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="0e245-1748">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="0e245-1748">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="0e245-1749">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-1749">Az.Monitor</span></span>
* <span data-ttu-id="0e245-1750">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="0e245-1750">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1751">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1751">Az.Network</span></span>
* <span data-ttu-id="0e245-1752">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="0e245-1752">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1753">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1753">Az.OperationalInsights</span></span>
* <span data-ttu-id="0e245-1754">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="0e245-1754">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="0e245-1755">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0e245-1755">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="0e245-1756">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="0e245-1756">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1757">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1757">Az.Resources</span></span>
* <span data-ttu-id="0e245-1758">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="0e245-1758">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="0e245-1759">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="0e245-1759">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="0e245-1760">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="0e245-1760">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="0e245-1761">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="0e245-1761">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1762">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1762">Az.Sql</span></span>
* <span data-ttu-id="0e245-1763">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="0e245-1763">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="0e245-1764">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="0e245-1764">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1765">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1765">Az.Websites</span></span>
* <span data-ttu-id="0e245-1766">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="0e245-1766">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="0e245-1767">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1767">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1768">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1768">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1769">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="0e245-1769">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="0e245-1770">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1770">Az.AnalysisServices</span></span>
<span data-ttu-id="0e245-1771">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="0e245-1771">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1772">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1772">Az.Compute</span></span>
* <span data-ttu-id="0e245-1773">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="0e245-1773">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="0e245-1774">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="0e245-1774">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="0e245-1775">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="0e245-1775">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1776">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1776">Az.RecoveryServices</span></span>
<span data-ttu-id="0e245-1777">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="0e245-1777">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1778">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1778">Az.Resources</span></span>
* <span data-ttu-id="0e245-1779">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="0e245-1779">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="0e245-1780">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="0e245-1780">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="0e245-1781">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="0e245-1781">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="0e245-1782">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="0e245-1782">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1783">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1783">Az.Sql</span></span>
* <span data-ttu-id="0e245-1784">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e245-1784">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="0e245-1785">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="0e245-1785">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="0e245-1786">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="0e245-1786">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="0e245-1787">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1787">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1788">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1788">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1789">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="0e245-1789">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="0e245-1790">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1790">Az.AnalysisServices</span></span>
* <span data-ttu-id="0e245-1791">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="0e245-1791">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1792">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1792">Az.RecoveryServices</span></span>
* <span data-ttu-id="0e245-1793">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="0e245-1793">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="0e245-1794">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1794">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1795">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1795">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1796">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="0e245-1796">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="0e245-1797">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1797">Update incorrect online help URLs</span></span>
* <span data-ttu-id="0e245-1798">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="0e245-1798">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="0e245-1799">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="0e245-1799">Az.Aks</span></span>
* <span data-ttu-id="0e245-1800">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1800">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="0e245-1801">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-1801">Az.Automation</span></span>
* <span data-ttu-id="0e245-1802">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="0e245-1802">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="0e245-1803">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1803">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="0e245-1804">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="0e245-1804">Az.Cdn</span></span>
* <span data-ttu-id="0e245-1805">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1805">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1806">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1806">Az.Compute</span></span>
* <span data-ttu-id="0e245-1807">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="0e245-1807">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="0e245-1808">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="0e245-1808">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="0e245-1809">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="0e245-1809">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="0e245-1810">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="0e245-1810">Az.ContainerRegistry</span></span>
* <span data-ttu-id="0e245-1811">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1811">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="0e245-1812">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="0e245-1812">Az.DataFactory</span></span>
* <span data-ttu-id="0e245-1813">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="0e245-1813">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1814">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1814">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-1815">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="0e245-1815">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="0e245-1816">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="0e245-1816">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="0e245-1817">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1817">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-1818">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1818">Az.IotHub</span></span>
* <span data-ttu-id="0e245-1819">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="0e245-1819">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="0e245-1820">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1820">Az.KeyVault</span></span>
* <span data-ttu-id="0e245-1821">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1821">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-1822">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1822">Az.Network</span></span>
* <span data-ttu-id="0e245-1823">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1823">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1824">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1824">Az.Resources</span></span>
* <span data-ttu-id="0e245-1825">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="0e245-1825">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="0e245-1826">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="0e245-1826">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="0e245-1827">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="0e245-1827">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="0e245-1828">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="0e245-1828">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="0e245-1829">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="0e245-1829">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="0e245-1830">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="0e245-1830">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="0e245-1831">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="0e245-1831">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-1832">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1832">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-1833">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="0e245-1833">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="0e245-1834">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="0e245-1834">Fix some error messages.</span></span>
* <span data-ttu-id="0e245-1835">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="0e245-1835">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="0e245-1836">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="0e245-1836">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="0e245-1837">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="0e245-1837">Az.SignalR</span></span>
* <span data-ttu-id="0e245-1838">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1838">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1839">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1839">Az.Sql</span></span>
* <span data-ttu-id="0e245-1840">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1840">Update incorrect online help URLs</span></span>
* <span data-ttu-id="0e245-1841">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="0e245-1841">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="0e245-1842">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="0e245-1842">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="0e245-1843">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="0e245-1843">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1844">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1844">Az.Storage</span></span>
* <span data-ttu-id="0e245-1845">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1845">Update incorrect online help URLs</span></span>
* <span data-ttu-id="0e245-1846">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="0e245-1846">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="0e245-1847">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="0e245-1847">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="0e245-1848">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="0e245-1848">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="0e245-1849">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="0e245-1849">Az.TrafficManager</span></span>
* <span data-ttu-id="0e245-1850">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1850">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1851">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1851">Az.Websites</span></span>
* <span data-ttu-id="0e245-1852">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="0e245-1852">Update incorrect online help URLs</span></span>
* <span data-ttu-id="0e245-1853">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="0e245-1853">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="0e245-1854">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="0e245-1854">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="0e245-1855">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="0e245-1855">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="0e245-1856">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1856">Az.Accounts</span></span>
* <span data-ttu-id="0e245-1857">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="0e245-1857">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-1858">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1858">Az.Compute</span></span>
* <span data-ttu-id="0e245-1859">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="0e245-1859">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="0e245-1860">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="0e245-1860">Updated the description of ID in help files</span></span>
* <span data-ttu-id="0e245-1861">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1861">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1862">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1862">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-1863">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="0e245-1863">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="0e245-1864">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="0e245-1864">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="0e245-1865">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="0e245-1865">Az.EventGrid</span></span>
* <span data-ttu-id="0e245-1866">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="0e245-1866">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="0e245-1867">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="0e245-1867">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="0e245-1868">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="0e245-1868">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="0e245-1869">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="0e245-1869">Event Time-To-Live,</span></span>
        - <span data-ttu-id="0e245-1870">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="0e245-1870">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="0e245-1871">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="0e245-1871">Dead letter endpoint.</span></span>
    - <span data-ttu-id="0e245-1872">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="0e245-1872">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="0e245-1873">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="0e245-1873">Event Time-To-Live,</span></span>
        - <span data-ttu-id="0e245-1874">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="0e245-1874">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="0e245-1875">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="0e245-1875">Dead letter endpoint.</span></span>
* <span data-ttu-id="0e245-1876">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="0e245-1876">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="0e245-1877">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="0e245-1877">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="0e245-1878">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1878">Az.IotHub</span></span>
* <span data-ttu-id="0e245-1879">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="0e245-1879">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="0e245-1880">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="0e245-1880">Az.LogicApp</span></span>
* <span data-ttu-id="0e245-1881">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="0e245-1881">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-1882">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1882">Az.Resources</span></span>
* <span data-ttu-id="0e245-1883">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="0e245-1883">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="0e245-1884">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="0e245-1884">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="0e245-1885">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0e245-1885">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="0e245-1886">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="0e245-1886">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="0e245-1887">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="0e245-1887">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="0e245-1888">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="0e245-1888">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="0e245-1889">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="0e245-1889">Az.SignalR</span></span>
* <span data-ttu-id="0e245-1890">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1890">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-1891">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1891">Az.Sql</span></span>
* <span data-ttu-id="0e245-1892">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="0e245-1892">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="0e245-1893">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1893">Az.Storage</span></span>
* <span data-ttu-id="0e245-1894">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="0e245-1894">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="0e245-1895">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="0e245-1895">New-AzStorageContext</span></span>
* <span data-ttu-id="0e245-1896">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="0e245-1896">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="0e245-1897">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="0e245-1897">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-1898">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1898">Az.Websites</span></span>
* <span data-ttu-id="0e245-1899">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="0e245-1899">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="0e245-1900">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1900">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="0e245-1901">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-1901">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="0e245-1902">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-1902">General</span></span>

- <span data-ttu-id="0e245-1903">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="0e245-1903">General Availability of Az Module</span></span>
- <span data-ttu-id="0e245-1904">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="0e245-1904">Online help for each module</span></span>
- <span data-ttu-id="0e245-1905">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="0e245-1905">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="0e245-1906">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="0e245-1906">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="0e245-1907">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1907">Az.Accounts</span></span>
- <span data-ttu-id="0e245-1908">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="0e245-1908">Changed from Az.Profile</span></span>
- <span data-ttu-id="0e245-1909">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="0e245-1909">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="0e245-1910">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-1910">Az.ApiManagement</span></span>
- <span data-ttu-id="0e245-1911">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="0e245-1911">Fixes for #7002</span></span>
- <span data-ttu-id="0e245-1912">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1912">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="0e245-1913">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="0e245-1913">Az.Batch</span></span>
- <span data-ttu-id="0e245-1914">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="0e245-1914">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="0e245-1915">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="0e245-1915">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="0e245-1916">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1916">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="0e245-1917">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="0e245-1917">Az.Billing</span></span>
- <span data-ttu-id="0e245-1918">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1918">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="0e245-1919">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1919">Az.CognitivServices</span></span>
- <span data-ttu-id="0e245-1920">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-1920">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="0e245-1921">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="0e245-1921">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="0e245-1922">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-1922">Az.ContainerInstance</span></span>
- <span data-ttu-id="0e245-1923">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="0e245-1923">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="0e245-1924">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="0e245-1924">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="0e245-1925">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1925">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1926">Az.DataLakeStore</span></span>
- <span data-ttu-id="0e245-1927">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1927">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="0e245-1928">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="0e245-1928">Az.Monitor</span></span>
- <span data-ttu-id="0e245-1929">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1929">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="0e245-1930">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="0e245-1930">Az.KeyVault</span></span>
- <span data-ttu-id="0e245-1931">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="0e245-1931">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="0e245-1932">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="0e245-1932">Az.MachineLearning</span></span>
- <span data-ttu-id="0e245-1933">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="0e245-1933">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="0e245-1934">Az.Media</span><span class="sxs-lookup"><span data-stu-id="0e245-1934">Az.Media</span></span>
- <span data-ttu-id="0e245-1935">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="0e245-1935">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="0e245-1936">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-1936">Az.Network</span></span>
<span data-ttu-id="0e245-1937">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="0e245-1937">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="0e245-1938">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0e245-1938">New cmdlets added:</span></span>
        - <span data-ttu-id="0e245-1939">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1939">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1940">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1940">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1941">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1941">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1942">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1942">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1943">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1943">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1944">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1944">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="0e245-1945">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1945">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="0e245-1946">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e245-1946">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="0e245-1947">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="0e245-1947">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="0e245-1948">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="0e245-1948">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="0e245-1949">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1949">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="0e245-1950">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="0e245-1950">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="0e245-1951">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1951">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="0e245-1952">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-1952">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="0e245-1953">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="0e245-1953">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="0e245-1954">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="0e245-1954">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="0e245-1955">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="0e245-1955">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="0e245-1956">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="0e245-1956">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="0e245-1957">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="0e245-1957">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="0e245-1958">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="0e245-1958">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="0e245-1959">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1959">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="0e245-1960">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-1960">Az.OperationalInsights</span></span>
- <span data-ttu-id="0e245-1961">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1961">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="0e245-1962">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="0e245-1962">Az.Profile</span></span>
- <span data-ttu-id="0e245-1963">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="0e245-1963">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1964">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1964">Az.RecoveryServices</span></span>
- <span data-ttu-id="0e245-1965">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1965">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="0e245-1966">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1966">Az.Resources</span></span>
- <span data-ttu-id="0e245-1967">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1967">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="0e245-1968">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-1968">Az.ServiceFabric</span></span>
- <span data-ttu-id="0e245-1969">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="0e245-1969">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="0e245-1970">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1970">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="0e245-1971">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="0e245-1971">Az.SIgnalR</span></span>
- <span data-ttu-id="0e245-1972">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="0e245-1972">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="0e245-1973">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1973">Az.Sql</span></span>
- <span data-ttu-id="0e245-1974">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="0e245-1974">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="0e245-1975">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="0e245-1975">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="0e245-1976">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1976">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="0e245-1977">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-1977">Az.Storage</span></span>
- <span data-ttu-id="0e245-1978">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1978">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="0e245-1979">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-1979">Az.Websites</span></span>
- <span data-ttu-id="0e245-1980">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="0e245-1980">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="0e245-1981">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-1981">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="0e245-1982">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-1982">General</span></span>

* <span data-ttu-id="0e245-1983">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="0e245-1983">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="0e245-1984">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-1984">Az.Compute</span></span>

* <span data-ttu-id="0e245-1985">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="0e245-1985">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="0e245-1986">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-1986">Az.DataLakeStore</span></span>

* <span data-ttu-id="0e245-1987">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="0e245-1987">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="0e245-1988">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="0e245-1988">Az.FrontDoor</span></span>

* <span data-ttu-id="0e245-1989">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="0e245-1989">Fixed some broken links</span></span>
    - <span data-ttu-id="0e245-1990">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="0e245-1990">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="0e245-1991">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="0e245-1991">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="0e245-1992">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="0e245-1992">Az.RecoveryServices</span></span>

* <span data-ttu-id="0e245-1993">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-1993">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="0e245-1994">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="0e245-1994">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="0e245-1995">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-1995">Az.Resources</span></span>

* <span data-ttu-id="0e245-1996">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="0e245-1996">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="0e245-1997">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="0e245-1997">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="0e245-1998">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-1998">Az.Sql</span></span>

* <span data-ttu-id="0e245-1999">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="0e245-1999">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="0e245-2000">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="0e245-2000">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="0e245-2001">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="0e245-2001">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="0e245-2002">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-2002">Az.Storage</span></span>

* <span data-ttu-id="0e245-2003">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="0e245-2003">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="0e245-2004">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="0e245-2004">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="0e245-2005">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-2005">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="0e245-2006">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="0e245-2006">Support Static Website configuration</span></span>
    - <span data-ttu-id="0e245-2007">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="0e245-2007">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="0e245-2008">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="0e245-2008">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="0e245-2009">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-2009">Az.Websites</span></span>

* <span data-ttu-id="0e245-2010">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="0e245-2010">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="0e245-2011">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="0e245-2011">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="0e245-2012">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-2012">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="0e245-2013">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-2013">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="0e245-2014">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="0e245-2014">Az.ApiManagement</span></span>
* <span data-ttu-id="0e245-2015">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="0e245-2015">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="0e245-2016">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="0e245-2016">Az.Automation</span></span>
* <span data-ttu-id="0e245-2017">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="0e245-2017">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="0e245-2018">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="0e245-2018">Added Update Management cmdlets</span></span>
* <span data-ttu-id="0e245-2019">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="0e245-2019">Added Source Control cmdlets</span></span>
* <span data-ttu-id="0e245-2020">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="0e245-2020">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="0e245-2021">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="0e245-2021">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="0e245-2022">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-2022">Az.Compute</span></span>
* <span data-ttu-id="0e245-2023">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="0e245-2023">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="0e245-2024">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="0e245-2024">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="0e245-2025">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-2025">Az.ContainerInstance</span></span>
* <span data-ttu-id="0e245-2026">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="0e245-2026">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="0e245-2027">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="0e245-2027">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="0e245-2028">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="0e245-2028">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="0e245-2029">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-2029">Az.Network</span></span>
* <span data-ttu-id="0e245-2030">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="0e245-2030">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="0e245-2031">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="0e245-2031">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="0e245-2032">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="0e245-2032">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="0e245-2033">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="0e245-2033">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="0e245-2034">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="0e245-2034">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="0e245-2035">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="0e245-2035">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="0e245-2036">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="0e245-2036">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="0e245-2037">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="0e245-2037">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="0e245-2038">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="0e245-2038">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="0e245-2039">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="0e245-2039">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="0e245-2040">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="0e245-2040">Az.Relay</span></span>
* <span data-ttu-id="0e245-2041">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="0e245-2041">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="0e245-2042">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-2042">Az.Resources</span></span>
* <span data-ttu-id="0e245-2043">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="0e245-2043">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="0e245-2044">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="0e245-2044">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="0e245-2045">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="0e245-2045">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="0e245-2046">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-2046">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-2047">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="0e245-2047">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="0e245-2048">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-2048">Az.Sql</span></span>
* <span data-ttu-id="0e245-2049">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-2049">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="0e245-2050">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-2050">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="0e245-2051">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-2051">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="0e245-2052">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-2052">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="0e245-2053">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="0e245-2053">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="0e245-2054">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="0e245-2054">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="0e245-2055">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="0e245-2055">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="0e245-2056">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="0e245-2056">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="0e245-2057">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="0e245-2057">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="0e245-2058">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="0e245-2058">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="0e245-2059">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="0e245-2059">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="0e245-2060">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="0e245-2060">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="0e245-2061">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="0e245-2061">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="0e245-2062">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="0e245-2062">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="0e245-2063">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="0e245-2063">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="0e245-2064">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="0e245-2064">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="0e245-2065">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="0e245-2065">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="0e245-2066">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-2066">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="0e245-2067">Geral</span><span class="sxs-lookup"><span data-stu-id="0e245-2067">General</span></span>
* <span data-ttu-id="0e245-2068">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="0e245-2068">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="0e245-2069">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="0e245-2069">Az.Profile</span></span>
* <span data-ttu-id="0e245-2070">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="0e245-2070">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="0e245-2071">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="0e245-2071">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="0e245-2072">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="0e245-2072">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="0e245-2073">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="0e245-2073">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="0e245-2074">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="0e245-2074">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="0e245-2075">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="0e245-2075">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="0e245-2076">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="0e245-2076">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-2077">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-2077">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-2078">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="0e245-2078">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-2079">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-2079">Az.Compute</span></span>
* <span data-ttu-id="0e245-2080">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="0e245-2080">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="0e245-2081">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="0e245-2081">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="0e245-2082">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="0e245-2082">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-2083">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-2083">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-2084">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="0e245-2084">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="0e245-2085">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="0e245-2085">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="0e245-2086">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="0e245-2086">Az.Insights</span></span>
* <span data-ttu-id="0e245-2087">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="0e245-2087">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="0e245-2088">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="0e245-2088">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="0e245-2089">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="0e245-2089">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="0e245-2090">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="0e245-2090">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-2091">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-2091">Az.Network</span></span>
* <span data-ttu-id="0e245-2092">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="0e245-2092">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="0e245-2093">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-2093">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="0e245-2094">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="0e245-2094">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="0e245-2095">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="0e245-2095">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="0e245-2096">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="0e245-2096">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="0e245-2097">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="0e245-2097">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="0e245-2098">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="0e245-2098">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="0e245-2099">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="0e245-2099">Az.PolicyInsights</span></span>
* <span data-ttu-id="0e245-2100">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="0e245-2100">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-2101">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-2101">Az.Resources</span></span>
* <span data-ttu-id="0e245-2102">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="0e245-2102">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="0e245-2103">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="0e245-2103">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="0e245-2104">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="0e245-2104">Az.ServiceBus</span></span>
* <span data-ttu-id="0e245-2105">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="0e245-2105">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="0e245-2106">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="0e245-2106">Az.ServiceFabric</span></span>
* <span data-ttu-id="0e245-2107">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="0e245-2107">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="0e245-2108">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="0e245-2108">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="0e245-2109">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="0e245-2109">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="0e245-2110">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="0e245-2110">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="0e245-2111">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="0e245-2111">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="0e245-2112">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-2112">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="0e245-2113">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="0e245-2113">Az.Profile</span></span>
* <span data-ttu-id="0e245-2114">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="0e245-2114">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="0e245-2115">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="0e245-2115">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-2116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-2116">Az.Compute</span></span>
* <span data-ttu-id="0e245-2117">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="0e245-2117">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="0e245-2118">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0e245-2118">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="0e245-2119">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="0e245-2119">Az.DataLakeStore</span></span>
* <span data-ttu-id="0e245-2120">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="0e245-2120">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="0e245-2121">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-2121">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="0e245-2122">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="0e245-2122">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="0e245-2123">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="0e245-2123">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="0e245-2124">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e245-2124">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-2125">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-2125">Az.Network</span></span>
* <span data-ttu-id="0e245-2126">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="0e245-2126">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="0e245-2127">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0e245-2127">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-2128">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-2128">Az.Resources</span></span>
* <span data-ttu-id="0e245-2129">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="0e245-2129">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="0e245-2130">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="0e245-2130">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="0e245-2131">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-2131">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="0e245-2132">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="0e245-2132">Azure.Storage</span></span>
* <span data-ttu-id="0e245-2133">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="0e245-2133">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="0e245-2134">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-2134">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="0e245-2135">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="0e245-2135">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="0e245-2136">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="0e245-2136">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="0e245-2137">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="0e245-2137">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="0e245-2138">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="0e245-2138">Az.CognitiveServices</span></span>
* <span data-ttu-id="0e245-2139">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="0e245-2139">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="0e245-2140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="0e245-2140">Az.Compute</span></span>
* <span data-ttu-id="0e245-2141">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="0e245-2141">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="0e245-2142">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="0e245-2142">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="0e245-2143">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="0e245-2143">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="0e245-2144">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="0e245-2144">Az.DataFactoryV2</span></span>
* <span data-ttu-id="0e245-2145">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="0e245-2145">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="0e245-2146">Az.Network</span><span class="sxs-lookup"><span data-stu-id="0e245-2146">Az.Network</span></span>
* <span data-ttu-id="0e245-2147">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="0e245-2147">Added NetworkProfile functionality.</span></span> <span data-ttu-id="0e245-2148">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="0e245-2148">new cmdlets added</span></span>
    - <span data-ttu-id="0e245-2149">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0e245-2149">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="0e245-2150">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0e245-2150">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="0e245-2151">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0e245-2151">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="0e245-2152">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="0e245-2152">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="0e245-2153">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-2153">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="0e245-2154">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-2154">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="0e245-2155">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="0e245-2155">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="0e245-2156">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="0e245-2156">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="0e245-2157">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="0e245-2157">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="0e245-2158">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="0e245-2158">Az.RedisCache</span></span>
* <span data-ttu-id="0e245-2159">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="0e245-2159">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="0e245-2160">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="0e245-2160">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="0e245-2161">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="0e245-2161">Az.Resources</span></span>
* <span data-ttu-id="0e245-2162">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0e245-2162">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="0e245-2163">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="0e245-2163">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="0e245-2164">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="0e245-2164">Az.Sql</span></span>
* <span data-ttu-id="0e245-2165">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="0e245-2165">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="0e245-2166">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="0e245-2166">Az.Websites</span></span>
* <span data-ttu-id="0e245-2167">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="0e245-2167">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="0e245-2168">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="0e245-2168">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="0e245-2169">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="0e245-2169">0.2.0 - September 2018</span></span>
 <span data-ttu-id="0e245-2170">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="0e245-2170">Initial Release</span></span>
