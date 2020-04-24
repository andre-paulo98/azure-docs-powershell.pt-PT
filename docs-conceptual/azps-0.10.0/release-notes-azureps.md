---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: c02cfaa7f7f39393f21cec31c5115f009381b19c
ms.sourcegitcommit: 4c61442a2df1cee633ce93cad9f6bc793803baa2
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/16/2020
ms.locfileid: "81446058"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="8b205-103">Notas de versão do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="8b205-103">Azure PowerShell release notes</span></span>
## <a name="0100-preview---april-2020"></a><span data-ttu-id="8b205-104">0.10.0-preview - Abril de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-104">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="8b205-105">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-105">General</span></span>
* <span data-ttu-id="8b205-106">Os módulos Az já estão disponíveis em pré-visualização no Azure Stack Hub.</span><span class="sxs-lookup"><span data-stu-id="8b205-106">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="8b205-107">Isto permite a compatibilidade entre plataformas diferentes com o Linux e macOS.</span><span class="sxs-lookup"><span data-stu-id="8b205-107">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="8b205-108">Agora, o Azure Stack Hub suporta o PowerShell Core com os módulos Az. Obtenha mais informações [aqui](https://aka.ms/az4AzureStack)</span><span class="sxs-lookup"><span data-stu-id="8b205-108">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="8b205-109">Os módulos Az suportam o perfil 2019-03-01-hybrid:</span><span class="sxs-lookup"><span data-stu-id="8b205-109">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="8b205-110">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8b205-110">Az.Billing</span></span>
  - <span data-ttu-id="8b205-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-111">Az.Compute</span></span>
  - <span data-ttu-id="8b205-112">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8b205-112">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="8b205-113">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-113">Az.EventHub</span></span>
  - <span data-ttu-id="8b205-114">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-114">Az.IotHub</span></span>
  - <span data-ttu-id="8b205-115">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-115">Az.KeyVault</span></span>
  - <span data-ttu-id="8b205-116">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-116">Az.Monitor</span></span>
  - <span data-ttu-id="8b205-117">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-117">Az.Network</span></span>
  - <span data-ttu-id="8b205-118">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-118">Az.Resources</span></span>
  - <span data-ttu-id="8b205-119">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-119">Az.Storage</span></span>
  - <span data-ttu-id="8b205-120">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-120">Az.Websites</span></span>
* <span data-ttu-id="8b205-121">Foram introduzidos três novos módulos do PowerShell para Az que funcionam com o Azure Stack Hub. São eles o Az.Databox, Az.IotHub e Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-121">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="8b205-122">Os comandos permanecem sensivelmente iguais, com pequenas alterações como, por exemplo, a alteração do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8b205-122">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="8b205-123">Veja uma ligação atualizada à documentação do PowerShell para o Azure Stack Hub [aqui](aka.ms/InstallASHPowerShell)</span><span class="sxs-lookup"><span data-stu-id="8b205-123">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](aka.ms/InstallASHPowerShell)</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-124">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-124">Az.Accounts</span></span>
* <span data-ttu-id="8b205-125">Atualização do ADAL para MSAL</span><span class="sxs-lookup"><span data-stu-id="8b205-125">Upgrade from ADAL to MSAL</span></span>


## <a name="370---march-2020"></a><span data-ttu-id="8b205-126">3.7.0 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-126">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-127">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-127">Az.Accounts</span></span>
* <span data-ttu-id="8b205-128">Foram corrigidos os parâmetros "Get-AzTenant"/"Get-AzDefault"/"Set-AzDefault" que emitiam uma NullReferenceException quando a sessão não estava iniciada [#10292]</span><span class="sxs-lookup"><span data-stu-id="8b205-128">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-129">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-129">Az.Compute</span></span>
* <span data-ttu-id="8b205-130">Foram adicionados os seguintes parâmetros ao cmdlet "New-AzDiskConfig":</span><span class="sxs-lookup"><span data-stu-id="8b205-130">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span> 
    - <span data-ttu-id="8b205-131">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="8b205-131">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="8b205-132">A propriedade Encryption foi permitida para o parâmetro Target do cmdlet "New-AzGalleryImageVersion".</span><span class="sxs-lookup"><span data-stu-id="8b205-132">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="8b205-133">Foi corrigido o problema de tempDisk para os cmdlets "Set-AzVmss" -Reimage e "Invoke-AzVMReimage".</span><span class="sxs-lookup"><span data-stu-id="8b205-133">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="8b205-134">[#11354]</span><span class="sxs-lookup"><span data-stu-id="8b205-134">[#11354]</span></span>
* <span data-ttu-id="8b205-135">Foi adicionado suporte aos cmdlets abaixo para a nova Extensão SAP</span><span class="sxs-lookup"><span data-stu-id="8b205-135">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="8b205-136">"Set-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8b205-136">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8b205-137">"Get-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8b205-137">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8b205-138">"Remove-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8b205-138">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="8b205-139">"Update-AzVMAEMExtension"</span><span class="sxs-lookup"><span data-stu-id="8b205-139">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="8b205-140">Foram corrigidos os erros em exemplos do documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-140">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="8b205-141">É apresentado o valor de cadeia exato para o PowerState da VM no formato de tabela.</span><span class="sxs-lookup"><span data-stu-id="8b205-141">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="8b205-142">"New-AzVmssConfig": foi corrigida a serialização da propriedade AutomaticRepairs quando a opção SinglePlacementGroup está desativada.</span><span class="sxs-lookup"><span data-stu-id="8b205-142">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="8b205-143">[#11257]</span><span class="sxs-lookup"><span data-stu-id="8b205-143">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-144">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-144">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-145">Atualização da versão do SDK .Net do ADF para 4.8.0</span><span class="sxs-lookup"><span data-stu-id="8b205-145">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="8b205-146">Foram adicionados parâmetros opcionais ao comando "Invoke-AzDataFactoryV2Pipeline" para suportar uma nova execução</span><span class="sxs-lookup"><span data-stu-id="8b205-146">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-147">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-147">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-148">Foi adicionada a descrição da alteração interruptiva para "Export-AzDataLakeStoreItem" e "Import-AzDataLakeStoreItem"</span><span class="sxs-lookup"><span data-stu-id="8b205-148">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="8b205-149">Foi adicionada a opção de codificação de bytes para "New-AzDataLakeStoreItem", "Add-AzDAtaLakeStoreItemContent" e "Get-AzDAtaLakeStoreItemContent"</span><span class="sxs-lookup"><span data-stu-id="8b205-149">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-150">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-150">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-151">É suportada a versão de TLS mínima suportada ao criar o cluster.</span><span class="sxs-lookup"><span data-stu-id="8b205-151">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-152">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-152">Az.IotHub</span></span>
* <span data-ttu-id="8b205-153">Foi adicionado suporte para gerir as definições distribuídas por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b205-153">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="8b205-154">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-154">New Cmdlets are:</span></span>
    - <span data-ttu-id="8b205-155">"Get-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="8b205-155">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="8b205-156">"Set-AzIotHubDistributedTracing"</span><span class="sxs-lookup"><span data-stu-id="8b205-156">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-157">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-157">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-158">Foram adicionados os atributos da alteração interruptiva a "New-AzKeyVault"</span><span class="sxs-lookup"><span data-stu-id="8b205-158">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-159">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-159">Az.Monitor</span></span>
* <span data-ttu-id="8b205-160">Foi atualizada a documentação de "New-AzScheduledQueryRuleLogMetricTrigger"</span><span class="sxs-lookup"><span data-stu-id="8b205-160">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-161">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-161">Az.Network</span></span>
* <span data-ttu-id="8b205-162">Foram atualizados os cmdlets para permitir VirtualHubVnetConnections entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="8b205-162">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="8b205-163">"New-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8b205-163">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8b205-164">"Update-AzVirtualHubVnetConnection"</span><span class="sxs-lookup"><span data-stu-id="8b205-164">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="8b205-165">"New-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="8b205-165">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="8b205-166">"Update-AzVirtualHub"</span><span class="sxs-lookup"><span data-stu-id="8b205-166">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="8b205-167">Foi removida a dependência do SDK do SQL Management</span><span class="sxs-lookup"><span data-stu-id="8b205-167">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-168">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-168">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-169">Mensagens de erro melhoradas</span><span class="sxs-lookup"><span data-stu-id="8b205-169">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-170">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-170">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-171">O Azure Site Recovery adicionou suporte para nova proteção e atualização das propriedades de VM para Máquinas Virtuais encriptadas em disco do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-171">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="8b205-172">Foi adicionada monitorização DR das propriedades VmwareToAzure ao Azure Site Recovery</span><span class="sxs-lookup"><span data-stu-id="8b205-172">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="8b205-173">O Azure Backup adicionou suporte para repetir a atualização de políticas para itens falhados.</span><span class="sxs-lookup"><span data-stu-id="8b205-173">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="8b205-174">O Azure Backup adicionou suporte para definições de exclusão do disco durante a cópia de segurança e o restauro.</span><span class="sxs-lookup"><span data-stu-id="8b205-174">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="8b205-175">O Azure Backup adicionou suporte para restaurar vários ficheiros/pastas no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="8b205-175">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="8b205-176">O Azure Backup adicionou suporte para o Resourcegroup especificado pelo utilizador durante a atualização da Política IaasVM</span><span class="sxs-lookup"><span data-stu-id="8b205-176">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-177">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-177">Az.Resources</span></span>
* <span data-ttu-id="8b205-178">Foi corrigido o parâmetro "Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType" para utilizar a apiVersion real dos recursos em vez da apiVersion predefinida [#11267]</span><span class="sxs-lookup"><span data-stu-id="8b205-178">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="8b205-179">Foi adicionado o registo de correlationId para cenários de erro</span><span class="sxs-lookup"><span data-stu-id="8b205-179">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="8b205-180">Pequena alteração à documentação referente a "Get-AzResourceLock".</span><span class="sxs-lookup"><span data-stu-id="8b205-180">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="8b205-181">Exemplo adicionado.</span><span class="sxs-lookup"><span data-stu-id="8b205-181">Added example.</span></span>
* <span data-ttu-id="8b205-182">Aspas com caráter de escape no valor de parâmetro "Get-AzADUser" [#11317]</span><span class="sxs-lookup"><span data-stu-id="8b205-182">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="8b205-183">Foram adicionados novos cmdlets aos Scripts de Implementação ("Get-AzDeploymentScript", "Get-AzDeploymentScriptLog", "Save-AzDeploymentScriptLog", "Remove-AzDeploymentScript")</span><span class="sxs-lookup"><span data-stu-id="8b205-183">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-184">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-184">Az.Sql</span></span>
* <span data-ttu-id="8b205-185">Foi adicionado um parâmetro secundário legível a "Invoke-AzSqlDatabaseFailover"</span><span class="sxs-lookup"><span data-stu-id="8b205-185">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="8b205-186">Foi adicionado o cmdlet "Disable-AzSqlServerActiveDirectoryOnlyAuthentication"</span><span class="sxs-lookup"><span data-stu-id="8b205-186">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="8b205-187">Classificação de sensibilidade guardada ao classificar as colunas na base de dados.</span><span class="sxs-lookup"><span data-stu-id="8b205-187">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="8b205-188">Az.Support</span><span class="sxs-lookup"><span data-stu-id="8b205-188">Az.Support</span></span>
* <span data-ttu-id="8b205-189">Disponibilidade geral do módulo "Az.Support"</span><span class="sxs-lookup"><span data-stu-id="8b205-189">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-190">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-190">Az.Websites</span></span>
* <span data-ttu-id="8b205-191">Foi adicionado suporte para utilizar Regras de Encaminhamento de Tráfego webapp através dos novos cmdlets abaixo</span><span class="sxs-lookup"><span data-stu-id="8b205-191">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="8b205-192">"Get-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8b205-192">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8b205-193">"Update-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8b205-193">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8b205-194">"Add-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8b205-194">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="8b205-195">"Remove-AzWebAppTrafficRouting"</span><span class="sxs-lookup"><span data-stu-id="8b205-195">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="8b205-196">3.6.1 - Março de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-196">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-197">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-197">Az.Accounts</span></span>
* <span data-ttu-id="8b205-198">Abrir a página de inquérito do Azure PowerShell em "Send-Feedback" [#11020]</span><span class="sxs-lookup"><span data-stu-id="8b205-198">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="8b205-199">Apresentar o URL de inquérito do Azure PowerShell em "Resolve-Error" [#11021]</span><span class="sxs-lookup"><span data-stu-id="8b205-199">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="8b205-200">Adicionada versão de Az em UserAgent</span><span class="sxs-lookup"><span data-stu-id="8b205-200">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8b205-201">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-201">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-202">Adicionado suporte para a obtenção e configuração do Domínio Personalizado no Ponto Final do DeveloperPortal [#11007]</span><span class="sxs-lookup"><span data-stu-id="8b205-202">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="8b205-203">"Export-AzApiManagementApi" Adicionado suporte para a transferência da definição da API no formato JSON [#9987]</span><span class="sxs-lookup"><span data-stu-id="8b205-203">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="8b205-204">"Import-AzApiManagementApi" Adicionado suporte para a importação da definição de OpenApi 3.0 a partir de documento JSON</span><span class="sxs-lookup"><span data-stu-id="8b205-204">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="8b205-205">"New-AzApiManagementIdentityProvider" e "Set-AzApiManagementIdentityProvider" Adicionado suporte para a configuração de "Inquilino de Início de Sessão" para Fornecedor de AAD B2C [#9784]</span><span class="sxs-lookup"><span data-stu-id="8b205-205">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-206">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-206">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-207">Adicionada referência a System.Buffers explicitamente em csproj e psd1.</span><span class="sxs-lookup"><span data-stu-id="8b205-207">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-208">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-208">Az.IotHub</span></span>
* <span data-ttu-id="8b205-209">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-209">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8b205-210">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-210">New Cmdlets are:</span></span>
    - <span data-ttu-id="8b205-211">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-211">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-212">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-212">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-213">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-213">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-214">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-214">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="8b205-215">Adicionado suporte para a gestão de módulos num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-215">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="8b205-216">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-216">New Cmdlets are:</span></span>
    - <span data-ttu-id="8b205-217">"Add-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8b205-217">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="8b205-218">"Get-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8b205-218">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="8b205-219">"Remove-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8b205-219">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="8b205-220">"Set-AzIotHubModule"</span><span class="sxs-lookup"><span data-stu-id="8b205-220">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="8b205-221">Adicionado cmdlet para obter a cadeia de ligação de um dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-221">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8b205-222">Adicionado cmdlet para obter a cadeia de ligação de um módulo num dispositivo IoT de destino num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-222">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="8b205-223">Adicionado suporte para obter/definir dispositivo principal de um dispositivo IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-223">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="8b205-224">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-224">New Cmdlets are:</span></span>
    - <span data-ttu-id="8b205-225">"Get-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="8b205-225">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="8b205-226">"Set-AzIotHubDeviceParent"</span><span class="sxs-lookup"><span data-stu-id="8b205-226">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="8b205-227">Adicionado suporte para gerir relações principal-subordinado de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b205-227">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-228">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-228">Az.Monitor</span></span>
* <span data-ttu-id="8b205-229">Corrigido o valor de saída de "Get-AzMetricDefinition" [#9714]</span><span class="sxs-lookup"><span data-stu-id="8b205-229">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-230">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-230">Az.Network</span></span>
* <span data-ttu-id="8b205-231">Sdk Sql Management atualizado.</span><span class="sxs-lookup"><span data-stu-id="8b205-231">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="8b205-232">Corrigido um problema de diferença de nomes na classe PrivateLinkServiceConnectionState.</span><span class="sxs-lookup"><span data-stu-id="8b205-232">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="8b205-233">Mapeamento do campo ActionsRequired para ActionRequired.</span><span class="sxs-lookup"><span data-stu-id="8b205-233">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="8b205-234">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="8b205-234">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-235">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-235">Az.Resources</span></span>
* <span data-ttu-id="8b205-236">Correção para erro de referência nula em "Get-AzRoleAssignment"</span><span class="sxs-lookup"><span data-stu-id="8b205-236">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="8b205-237">Comutadores "-Force" e "-PassThru" marcados como opcionais em "Remove-AzADGroup" [#10849]</span><span class="sxs-lookup"><span data-stu-id="8b205-237">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="8b205-238">Corrigido problema em que "MailNickname" não devolve "Remove-AzADGroup" [#11167]</span><span class="sxs-lookup"><span data-stu-id="8b205-238">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="8b205-239">Corrigido problema em que a operação de pipe "Remove-AzADGroup" não funciona [#11171]</span><span class="sxs-lookup"><span data-stu-id="8b205-239">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="8b205-240">Correção para erro de referência nula em GetAzureRoleAssignmentCommand</span><span class="sxs-lookup"><span data-stu-id="8b205-240">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="8b205-241">Adicionados atributos de alterações interruptivas para futuras alterações a cmdlets de política</span><span class="sxs-lookup"><span data-stu-id="8b205-241">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="8b205-242">"Get-AzResourceGroup" atualizado para realizar filtragem de etiqueta de grupo de recursos no lado do servidor</span><span class="sxs-lookup"><span data-stu-id="8b205-242">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="8b205-243">Cmdlets Tag alargados para accept -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-243">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="8b205-244">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-244">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8b205-245">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-245">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="8b205-246">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-246">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="8b205-247">Adicionado cmdlet Tag novo</span><span class="sxs-lookup"><span data-stu-id="8b205-247">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="8b205-248">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-248">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="8b205-249">ScopedDeployment trazido de SDK 3.3.0</span><span class="sxs-lookup"><span data-stu-id="8b205-249">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-250">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-250">Az.Sql</span></span>
* <span data-ttu-id="8b205-251">Adicionado PublicNetworkAccess a "New-AzSqlServer" e "Set-AzSqlServer"</span><span class="sxs-lookup"><span data-stu-id="8b205-251">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="8b205-252">Adicionado suporte para configuração de cópia de segurança de Retenção de Longo Prazo para Bases de Dados Geridas</span><span class="sxs-lookup"><span data-stu-id="8b205-252">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="8b205-253">Política Get/Set numa base de dados gerida</span><span class="sxs-lookup"><span data-stu-id="8b205-253">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="8b205-254">Obter cópia(s) de segurança LTR por base de dados gerida, por instância gerida ou por localização</span><span class="sxs-lookup"><span data-stu-id="8b205-254">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="8b205-255">Remover uma cópia de segurança LTR</span><span class="sxs-lookup"><span data-stu-id="8b205-255">Remove an LTR backup</span></span>
    - <span data-ttu-id="8b205-256">Restaurar uma cópia de segurança LTR para criar uma base de dados gerida nova</span><span class="sxs-lookup"><span data-stu-id="8b205-256">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="8b205-257">Adicionado MinimalTlsVersion a New-AzSqlServer e Set-AzSqlServer</span><span class="sxs-lookup"><span data-stu-id="8b205-257">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="8b205-258">Adicionado MinimalTlsVersion a New-AzSqlInstance e Set-AzSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-258">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="8b205-259">Versão de SDK SQL atualizada para Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-259">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-260">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-260">Az.Storage</span></span>
* <span data-ttu-id="8b205-261">AllowProtectedAppendWrite suportada em ImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-261">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="8b205-262">"Set-AzRmStorageContainerImmutabilityPolicy"</span><span class="sxs-lookup"><span data-stu-id="8b205-262">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="8b205-263">Adicionada uma mensagem de aviso de alteração interruptiva para alteração do tipo AzureStorageTable numa futura versão</span><span class="sxs-lookup"><span data-stu-id="8b205-263">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="8b205-264">"New-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="8b205-264">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="8b205-265">"Get-AzStorageTable"</span><span class="sxs-lookup"><span data-stu-id="8b205-265">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-266">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-266">Az.Websites</span></span>
* <span data-ttu-id="8b205-267">Adicionado o parâmetro Tag para "New-AzAppServicePlan" e "Set-AzAppServicePlan"</span><span class="sxs-lookup"><span data-stu-id="8b205-267">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="8b205-268">Paragem da execução de cmdlet caso seja emitida uma exceção ao adicionar um domínio personalizado a um site</span><span class="sxs-lookup"><span data-stu-id="8b205-268">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="8b205-269">Adicionado suporte para a realização de operações para Serviços de Aplicações em grupos de recursos diferentes do Plano do Serviço de Aplicações</span><span class="sxs-lookup"><span data-stu-id="8b205-269">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="8b205-270">Aplicada restrição de acesso a WebApp/Função em diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="8b205-270">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="8b205-271">Corrigido problema para definir os nomes de anfitrião personalizados para WebAppSlots</span><span class="sxs-lookup"><span data-stu-id="8b205-271">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="8b205-272">3.5.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-272">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-273">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-273">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-274">Telemetria do lado do cliente atualizada.</span><span class="sxs-lookup"><span data-stu-id="8b205-274">Updated client side telemetry.</span></span>
* <span data-ttu-id="8b205-275">O Az.IotHub adicionou cmdlets para suportar a gestão de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8b205-275">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="8b205-276">O Az.SqlVirtualMachine adicionou cmdlets ao Serviço de Escuta do Grupo de Disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b205-276">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-277">Az.Accounts</span></span>
* <span data-ttu-id="8b205-278">SubscriptionId, TenantId e tempo de execução adicionados aos dados de telemetria do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="8b205-278">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-279">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-279">Az.Automation</span></span>
* <span data-ttu-id="8b205-280">Foi corrigido o erro no Exemplo 1 na documentação de referência de "New-AzAutomationSoftwareUpdateConfiguration"</span><span class="sxs-lookup"><span data-stu-id="8b205-280">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-281">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-281">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-282">SDK atualizado para a versão 7.0</span><span class="sxs-lookup"><span data-stu-id="8b205-282">Updated SDK to 7.0</span></span>
* <span data-ttu-id="8b205-283">Mensagem de erro melhorada quando o servidor responde ao corpo vazio</span><span class="sxs-lookup"><span data-stu-id="8b205-283">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-284">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-284">Az.Compute</span></span>
* <span data-ttu-id="8b205-285">Valor vazio permitido para ProximityPlacementGroupId durante a atualização</span><span class="sxs-lookup"><span data-stu-id="8b205-285">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-286">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-286">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-287">Cmdlet adicionado para obter definições de regras geridas que podem ser utilizadas na WAF</span><span class="sxs-lookup"><span data-stu-id="8b205-287">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-288">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-288">Az.IotHub</span></span>
* <span data-ttu-id="8b205-289">Suporte adicionado para gerir dispositivos num Hub IoT.</span><span class="sxs-lookup"><span data-stu-id="8b205-289">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="8b205-290">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-290">New Cmdlets are:</span></span>
    - <span data-ttu-id="8b205-291">"Add-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-291">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-292">"Get-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-292">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-293">"Remove-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-293">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="8b205-294">"Set-AzIotHubDevice"</span><span class="sxs-lookup"><span data-stu-id="8b205-294">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-295">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-295">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-296">Texto duplicado fixo para Add-AzKeyVaultKey.md</span><span class="sxs-lookup"><span data-stu-id="8b205-296">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-297">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-297">Az.Monitor</span></span>
* <span data-ttu-id="8b205-298">Descrição fixa do cmdlet Get-AzLog.</span><span class="sxs-lookup"><span data-stu-id="8b205-298">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="8b205-299">Foi adicionado um novo parâmetro chamado ActionGroupId ao comando "New-AzMetricAlertRuleV2".</span><span class="sxs-lookup"><span data-stu-id="8b205-299">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="8b205-300">O utilizador pode fornecer ActionGroupId(string) ou ActionGorup(ActivityLogAlertActionGroup).</span><span class="sxs-lookup"><span data-stu-id="8b205-300">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-301">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-301">Az.Network</span></span>
* <span data-ttu-id="8b205-302">Foi adicionada uma nota de parâmetro adicional para o parâmetro "-EnableProxyProtocol" para o cmdlet "New-AzPrivateLinkService".</span><span class="sxs-lookup"><span data-stu-id="8b205-302">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="8b205-303">Exemplo de FilterData fixo em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="8b205-303">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8b205-304">Exemplo de Captura de Pacotes adicionado para capturar todos os pacotes internos e externos em Start-AzVirtualNetworkGatewayConnectionPacketCapture.md e Start-AzVirtualnetworkGatewayPacketCapture.md.</span><span class="sxs-lookup"><span data-stu-id="8b205-304">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="8b205-305">Política do Azure Firewall suportada em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="8b205-305">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="8b205-306">Não foram adicionados novos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8b205-306">No new cmdlets are added.</span></span> <span data-ttu-id="8b205-307">Simplificação da restrição da política de firewall em firewalls VNet</span><span class="sxs-lookup"><span data-stu-id="8b205-307">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-308">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-308">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-309">Suporte adicionado da funcionalidade Restaurar como ficheiros para Bases de Dados SQL.</span><span class="sxs-lookup"><span data-stu-id="8b205-309">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-310">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-310">Az.Resources</span></span>
* <span data-ttu-id="8b205-311">Cmdlets de implementação de modelos refatorizados</span><span class="sxs-lookup"><span data-stu-id="8b205-311">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="8b205-312">Foram adicionados novos cmdlets para gerir implementações no grupo de gestão: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="8b205-312">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="8b205-313">Foram adicionados novos cmdlets para gerir implementações no inquilino: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="8b205-313">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="8b205-314">Cmdlets \*-AzDeployment refatorizados para trabalhar especificamente no âmbito da subscrição</span><span class="sxs-lookup"><span data-stu-id="8b205-314">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="8b205-315">Foram criados aliases \*-AzSubscriptionDeployment para os cmdlets \*-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="8b205-315">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="8b205-316">"Update-AzADApplication" fixo quando o parâmetro "AvailableToOtherTenants" não está definido</span><span class="sxs-lookup"><span data-stu-id="8b205-316">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="8b205-317">ApplicationObjectWithoutCredentialParameterSet removido para evitar AmbiguousParameterSetException.</span><span class="sxs-lookup"><span data-stu-id="8b205-317">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="8b205-318">Ficheiros de ajuda regenerados</span><span class="sxs-lookup"><span data-stu-id="8b205-318">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-319">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-319">Az.Sql</span></span>
* <span data-ttu-id="8b205-320">Suporte adicionado para restauro para um ponto anterior no tempo entre subscrições nas Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="8b205-320">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="8b205-321">Suporte adicionado para alterar a geração de hardware das Instâncias Geridas de SQL existentes</span><span class="sxs-lookup"><span data-stu-id="8b205-321">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="8b205-322">Exemplos de ajuda "Update-AzSqlServerVulnerabilityAssessmentSetting" fixos: saída do parâmetro/propriedade - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="8b205-322">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8b205-323">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8b205-323">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8b205-324">Cmdlets adicionados para o Serviço de Escuta do Grupo de Disponibilidade</span><span class="sxs-lookup"><span data-stu-id="8b205-324">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8b205-325">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8b205-325">Az.StorageSync</span></span>
* <span data-ttu-id="8b205-326">Conjuntos de carateres suportados atualizados em "Invoke-AzStorageSyncCompatibilityCheck".</span><span class="sxs-lookup"><span data-stu-id="8b205-326">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="8b205-327">3.4.0 - Fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-327">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-328">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-328">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-329">Versão inicial Az.CosmosDB 0.1.0 lançada</span><span class="sxs-lookup"><span data-stu-id="8b205-329">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="8b205-330">Foi adicionado suporte para Az.Network ConnectionMonitor V2</span><span class="sxs-lookup"><span data-stu-id="8b205-330">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-331">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-331">Az.Accounts</span></span>
* <span data-ttu-id="8b205-332">Foi desativada a gravação automática de contexto quando AzureRmContext.json não está disponível</span><span class="sxs-lookup"><span data-stu-id="8b205-332">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="8b205-333">Atualização da referência ao Azure Powershell Common para a pré-visualização 1.3.5</span><span class="sxs-lookup"><span data-stu-id="8b205-333">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8b205-334">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-334">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-335">**Get-AzApiManagementApiSchema** Foi corrigido ao obter Open-Api Schema associado a uma API   https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="8b205-335">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="8b205-336">**New-AzApiManagementProduct**\* e **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="8b205-336">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="8b205-337">Foi corrigida a documentação para https://github.com/Azure/azure-powershell/issues/10472</span><span class="sxs-lookup"><span data-stu-id="8b205-337">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="8b205-338">**Set-AzApiManagementApi** Exemplo adicionado para mostrar como atualizar o ServiceUrl com o cmdlet</span><span class="sxs-lookup"><span data-stu-id="8b205-338">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-339">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-339">Az.Compute</span></span>
* <span data-ttu-id="8b205-340">Foi limitado o número de estados de VM a 100 para evitar limitações quando Get-AzVM-Status é executado sem o nome da VM.</span><span class="sxs-lookup"><span data-stu-id="8b205-340">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="8b205-341">Foi adicionado o cmdlet Update-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="8b205-341">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="8b205-342">Foram adicionados os parâmetros EncryptionType e DiskEncryptionSetId aos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-342">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="8b205-343">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-343">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="8b205-344">Foi adicionado o parâmetro ColocationStatus ao cmdlet Get-AzProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="8b205-344">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-345">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-345">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-346">Atualização do SDK .NET do ADF para a versão 4.7.0</span><span class="sxs-lookup"><span data-stu-id="8b205-346">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8b205-347">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8b205-347">Az.DeploymentManager</span></span>
* <span data-ttu-id="8b205-348">Adiciona operações LIST para os recursos</span><span class="sxs-lookup"><span data-stu-id="8b205-348">Adds LIST operations for resources</span></span>
* <span data-ttu-id="8b205-349">Adiciona a capacidade de realizar operações nos passos de Verificação de Estado de Funcionamento</span><span class="sxs-lookup"><span data-stu-id="8b205-349">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-350">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-350">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-351">Foi corrigido o erro do documento de New-AzHDInsightCluster.</span><span class="sxs-lookup"><span data-stu-id="8b205-351">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-352">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-352">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-353">Foi adicionado o alias do Nome ao atributo VaultName para tornar Remove-AzureKeyVault consistente com New-AzureKeyVault.</span><span class="sxs-lookup"><span data-stu-id="8b205-353">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-354">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-354">Az.Network</span></span>
* <span data-ttu-id="8b205-355">Foi adicionado um novo exemplo a Set-AzNetworkWatcherConfigFlowLog.md para demonstrar o cenário de desativação da Análise de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="8b205-355">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="8b205-356">Foi adicionado suporte para atribuir a configuração IP de gestão ao Azure Firewall, uma sub-rede dedicada e IP Público que a firewall utilizará no tráfego de gestão</span><span class="sxs-lookup"><span data-stu-id="8b205-356">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="8b205-357">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-357">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8b205-358">Foi adicionado o parâmetro -ManagementPublicIpAddress (não obrigatório) que aceita um objeto de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="8b205-358">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="8b205-359">Foi adicionado o método SetManagementIpConfiguration no objeto de firewall. Requer uma sub-rede e um endereço IP Público como entrada. O nome da sub-rede tem de ser "AzureFirewallManagementSubnet"</span><span class="sxs-lookup"><span data-stu-id="8b205-359">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="8b205-360">Foram corrigidos os exemplos de Get-AzNetworkSecurityGroup para mostrar exemplos de NSGs em vez de interfaces de rede.</span><span class="sxs-lookup"><span data-stu-id="8b205-360">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="8b205-361">Foi corrigido um erro no comando New-AzVpnSite que estava a impedir o ID do recurso de concluir um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8b205-361">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="8b205-362">Foi adicionado suporte para a Configuração do URL em Reescrever Conjunto de Ações de Regras no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8b205-362">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="8b205-363">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-363">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-364">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-364">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="8b205-365">Foram atualizados cmdlets com o parâmetro opcional - UrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-365">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="8b205-366">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8b205-366">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="8b205-367">Foi adicionado suporte para os recursos do NetworkWatcher ConnectionMonitor versão 2</span><span class="sxs-lookup"><span data-stu-id="8b205-367">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-368">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-368">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-369">Foi adicionado suporte para avaliar a conformidade antes de determinar o recurso a remediar</span><span class="sxs-lookup"><span data-stu-id="8b205-369">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="8b205-370">Foi adicionado o parâmetro "-ResourceDiscoverMode" a Start-AzPolicyRemediation</span><span class="sxs-lookup"><span data-stu-id="8b205-370">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="8b205-371">Foi adicionado o cmdlet Get-AzPolicyMetadata para obter os recursos de metadados da política</span><span class="sxs-lookup"><span data-stu-id="8b205-371">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="8b205-372">Get-AzPolicyState e Get-AzPolicyStateSummary atualizados para a versão da API 2019-10-01</span><span class="sxs-lookup"><span data-stu-id="8b205-372">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-373">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-373">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-374">Foi adicionado suporte do Azure Site Recovery para remover um disco replicado.</span><span class="sxs-lookup"><span data-stu-id="8b205-374">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="8b205-375">O Azure Backup adicionou suporte para adicionar etiquetas ao criar um Cofre dos Serviços de Recuperação.</span><span class="sxs-lookup"><span data-stu-id="8b205-375">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-376">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-376">Az.Resources</span></span>
* <span data-ttu-id="8b205-377">-Scope foi tornado opcional nos cmdlets \*-AzPolicyAssignment com subscrição de contexto predefinida</span><span class="sxs-lookup"><span data-stu-id="8b205-377">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="8b205-378">Foram adicionados exemplos de criação de ADServicePrincipal com credenciais de palavras-passe e chaves</span><span class="sxs-lookup"><span data-stu-id="8b205-378">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-379">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-379">Az.Sql</span></span>
<span data-ttu-id="8b205-380">Foi corrigido o cmdlet New-AzSqlDatabaseSecondary para verificar a existência de PartnerDatabaseName em vez da existência de DatabaseName.</span><span class="sxs-lookup"><span data-stu-id="8b205-380">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-381">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-381">Az.Storage</span></span>
* <span data-ttu-id="8b205-382">Foi definido o suporte de Tipo de Chave de Encriptação na Tabela/Fila em Criar Conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b205-382">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="8b205-383">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-383">New-AzStorageAccount</span></span>
* <span data-ttu-id="8b205-384">Será apresentado RequestId quando StorageException não tiver ExtendedErrorInformation</span><span class="sxs-lookup"><span data-stu-id="8b205-384">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="8b205-385">Foi corrigido o exemplo 6 do cmdlet Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-385">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-386">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-386">Az.Websites</span></span>
* <span data-ttu-id="8b205-387">Set-AzWebapp e Set-AzWebappSlot suportam as propriedades AlwaysOn, MinTls e FtpsState</span><span class="sxs-lookup"><span data-stu-id="8b205-387">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="8b205-388">Foi corrigido o problema em que a definição de HttpsOnly, juntamente com a alteração de AppservicePlan ao utilizar o único comando Set-AzWebApp, estava a repor HttpsOnly para o valor predefinido</span><span class="sxs-lookup"><span data-stu-id="8b205-388">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="8b205-389">3.3.0 – janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="8b205-389">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-390">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-390">Az.Accounts</span></span>
* <span data-ttu-id="8b205-391">Add-AzEnvironment e Set-AzEnvironment foram atualizados para aceitar os parâmetros AzureAttestationServiceEndpointResourceId e AzureAttestationServiceEndpointSuffix</span><span class="sxs-lookup"><span data-stu-id="8b205-391">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-392">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-392">Az.Cdn</span></span>
* <span data-ttu-id="8b205-393">Apresentação dos detalhes da resposta de erro no cmdlet New-AzCdnEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-393">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-394">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-394">Az.Compute</span></span>
* <span data-ttu-id="8b205-395">Correção do cmdlet Set-AzVMCustomScriptExtension para uma VM com disco OD gerido sem perfil de SO.</span><span class="sxs-lookup"><span data-stu-id="8b205-395">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="8b205-396">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-396">Az.ContainerInstance</span></span>
* <span data-ttu-id="8b205-397">Foram corrigidos os nomes de parâmetros utilizados pelo exemplo de New-AzContainerGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-397">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8b205-398">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8b205-398">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8b205-399">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8b205-399">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8b205-400">Obter o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-400">Get the Edge Storage Container</span></span>
* <span data-ttu-id="8b205-401">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8b205-401">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8b205-402">Criar novo Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-402">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="8b205-403">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8b205-403">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8b205-404">Remover o Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-404">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="8b205-405">Foi adicionado o cmdlet "Invoke-AzDataBoxEdgeStorageContainer"</span><span class="sxs-lookup"><span data-stu-id="8b205-405">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="8b205-406">Invocar ação para atualizar os dados no Contentor de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-406">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="8b205-407">Foi adicionado o cmdlet "Get-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8b205-407">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8b205-408">Obter a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-408">Get the Edge Storage Account</span></span>
* <span data-ttu-id="8b205-409">Foi adicionado o cmdlet "New-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8b205-409">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8b205-410">Criar nova Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-410">Create new Edge Storage Account</span></span>
* <span data-ttu-id="8b205-411">Foi adicionado o cmdlet "Remove-AzDataBoxEdgeStorageAccount"</span><span class="sxs-lookup"><span data-stu-id="8b205-411">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="8b205-412">Remover a Conta de Armazenamento Edge</span><span class="sxs-lookup"><span data-stu-id="8b205-412">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="8b205-413">Invocar o cmdlet "Invoke-AzDataBoxEdgeShare"</span><span class="sxs-lookup"><span data-stu-id="8b205-413">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="8b205-414">Invocar ação para atualizar os dados na partilha</span><span class="sxs-lookup"><span data-stu-id="8b205-414">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="8b205-415">Foi adicionado o cmdlet "Set-AzDataBoxEdgeStorageAccountCredential"</span><span class="sxs-lookup"><span data-stu-id="8b205-415">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="8b205-416">Definição de AzDataBoxEdgeStorageAccountCredential</span><span class="sxs-lookup"><span data-stu-id="8b205-416">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-417">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-417">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-418">Adição das propriedades AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId e VersionStatus para o cmd Get-AzDataFactoryV2IntegrationRuntime</span><span class="sxs-lookup"><span data-stu-id="8b205-418">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="8b205-419">Atualização do SDK .NET do ADF para a versão 4.6.0</span><span class="sxs-lookup"><span data-stu-id="8b205-419">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="8b205-420">Adição do parâmetro "PublicIPs" para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a criação de Azure-SSIS IR com endereços IP públicos estáticos.</span><span class="sxs-lookup"><span data-stu-id="8b205-420">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="8b205-421">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="8b205-421">Az.DevTestLabs</span></span>
* <span data-ttu-id="8b205-422">Remoção da ligação quebrada em Get-AzDtlAllowedVMSizesPolicy.md</span><span class="sxs-lookup"><span data-stu-id="8b205-422">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-423">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-423">Az.EventHub</span></span>
* <span data-ttu-id="8b205-424">Correção do problema 10634: Correção da referência de objeto nulo para remover eventhubnamespace</span><span class="sxs-lookup"><span data-stu-id="8b205-424">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-425">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-425">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-426">Correção do erro Invoke-AzHDInsightHiveJob.md.</span><span class="sxs-lookup"><span data-stu-id="8b205-426">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8b205-427">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8b205-427">Az.MachineLearning</span></span>
* <span data-ttu-id="8b205-428">Foram removidos os cmdlets abaixo porque MachineLearningCompute já não está disponível</span><span class="sxs-lookup"><span data-stu-id="8b205-428">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="8b205-429">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8b205-429">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="8b205-430">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="8b205-430">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="8b205-431">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8b205-431">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="8b205-432">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8b205-432">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="8b205-433">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="8b205-433">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="8b205-434">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="8b205-434">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="8b205-435">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="8b205-435">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-436">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-436">Az.Network</span></span>
* <span data-ttu-id="8b205-437">Atualização da dependência de Microsoft.Azure.Management.SQL da versão 1.36-preview para 1.37-preview</span><span class="sxs-lookup"><span data-stu-id="8b205-437">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-438">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-438">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-439">Alteração do Azure Site Recovery para suportar VMs de disco gerido com encriptação inativa com chaves geridas pelo cliente para o fornecedor do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-439">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="8b205-440">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-440">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8b205-441">Suporte do Azure Site Recovery para encriptar o disco de entrada e definir o ID como entrada opcional ao nível do disco para ativar a proteção de VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-441">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="8b205-442">Suporte do Azure Site Recovery para atualizar o item protegido por replicação com encriptação de discos e definir o mapa para HyperV para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-442">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-443">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-443">Az.Resources</span></span>
* <span data-ttu-id="8b205-444">Correção de um erro no documento de ajuda de "Remove-AzTag".</span><span class="sxs-lookup"><span data-stu-id="8b205-444">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-445">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-445">Az.Sql</span></span>
* <span data-ttu-id="8b205-446">Correção da funcionalidade dos cmdlets de linha de base do conjunto de avaliação de vulnerabilidades para funcionar na base de dados mestre da base de dados do Azure e limitá-la nas bases de dados do sistema de instância gerida</span><span class="sxs-lookup"><span data-stu-id="8b205-446">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="8b205-447">Correção de um erro ao criar o grupo de ativação pós-falha de instância SQL</span><span class="sxs-lookup"><span data-stu-id="8b205-447">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="8b205-448">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8b205-448">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="8b205-449">Adição de DR como um novo tipo de Licença válido</span><span class="sxs-lookup"><span data-stu-id="8b205-449">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-450">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-450">Az.Storage</span></span>
* <span data-ttu-id="8b205-451">Adição de uma mensagem de aviso de alteração interruptiva para alteração do valor de DefaultAction numa futura versão</span><span class="sxs-lookup"><span data-stu-id="8b205-451">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="8b205-452">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-452">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="8b205-453">Suporte para obter a hora da última sincronização da conta de armazenamento ao executar get-AzureRMStorageAccount com o parâmetro -IncludeGeoReplicationStats</span><span class="sxs-lookup"><span data-stu-id="8b205-453">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="8b205-454">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-454">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="8b205-455">3.2.0 - Dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-455">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="8b205-456">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-456">General</span></span>
* <span data-ttu-id="8b205-457">Atualização das referências em .psd1 para utilizar o caminho relativo para todos os módulos</span><span class="sxs-lookup"><span data-stu-id="8b205-457">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-458">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-458">Az.Accounts</span></span>
* <span data-ttu-id="8b205-459">Definição do UserAgent correto para telemetria do lado do cliente para a pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="8b205-459">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="8b205-460">Apresentação de mensagem de erro amigável de utilizador quando o contexto é nulo na pré-visualização do Az 4.0</span><span class="sxs-lookup"><span data-stu-id="8b205-460">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8b205-461">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-461">Az.Batch</span></span>
* <span data-ttu-id="8b205-462">Correção do problema [10602](https://github.com/Azure/azure-powershell/issues/10602), em que **New-AzBatchPool** não enviava corretamente "VirtualMachineConfiguration.ContainerConfiguration" ou "VirtualMachineConfiguration.DataDisks" para o servidor.</span><span class="sxs-lookup"><span data-stu-id="8b205-462">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-463">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-463">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-464">Atualização do SDK .NET do ADF para a versão 4.5.0</span><span class="sxs-lookup"><span data-stu-id="8b205-464">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-465">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-465">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-466">Adição do suporte de exclusão de regras geridas pela WAF</span><span class="sxs-lookup"><span data-stu-id="8b205-466">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="8b205-467">Adição de SocketAddr ao preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="8b205-467">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8b205-468">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8b205-468">Az.HealthcareApis</span></span>
* <span data-ttu-id="8b205-469">Processamento de Exceções</span><span class="sxs-lookup"><span data-stu-id="8b205-469">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-470">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-470">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-471">Correção do erro em que era acedido um valor potencialmente não definido</span><span class="sxs-lookup"><span data-stu-id="8b205-471">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="8b205-472">Gestão de Certificados de Criptografia de Curva Elíptica</span><span class="sxs-lookup"><span data-stu-id="8b205-472">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="8b205-473">Adicionado suporte para especificar a Curva das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="8b205-473">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-474">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-474">Az.Monitor</span></span>
* <span data-ttu-id="8b205-475">Adição de um argumento opcional ao comando Adicionar Definições de Diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8b205-475">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="8b205-476">Um argumento de opção que, se estiver presente, indica que a exportação para o Log Analytics deve ser feita para um esquema fixo (também conhecido como</span><span class="sxs-lookup"><span data-stu-id="8b205-476">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="8b205-477">tipo de dados dedicado)</span><span class="sxs-lookup"><span data-stu-id="8b205-477">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-478">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-478">Az.Network</span></span>
* <span data-ttu-id="8b205-479">Suporte para IpGroups na aplicação AzureFirewall, Nat e Regras de Rede.</span><span class="sxs-lookup"><span data-stu-id="8b205-479">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-480">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-480">Az.Resources</span></span>
* <span data-ttu-id="8b205-481">Correção de um problema em que a implementação do modelo não consegue ler um parâmetro se o nome estiver em conflito com um nome de parâmetro incorporado.</span><span class="sxs-lookup"><span data-stu-id="8b205-481">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="8b205-482">Os cmdlets da política foram atualizados para utilizar a nova versão de API 2019-09-01 que introduz suporte de agrupamento nas definições do conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="8b205-482">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-483">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-483">Az.Sql</span></span>
* <span data-ttu-id="8b205-484">Criação do armazenamento atualizada na ativação automática da Avaliação de Vulnerabilidades para StorageV2</span><span class="sxs-lookup"><span data-stu-id="8b205-484">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-485">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-485">Az.Storage</span></span>
* <span data-ttu-id="8b205-486">Suporte para gerar um token de SAS baseado na Identidade do Blob/Contentor com Contexto de Armazenamento baseado na autenticação OAuth</span><span class="sxs-lookup"><span data-stu-id="8b205-486">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="8b205-487">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="8b205-487">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="8b205-488">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8b205-488">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="8b205-489">Suporte para revogar as Chaves de Delegação do Utilizador da Conta de Armazenamento, pelo que todos os tokens de SAS da identidade são revogados</span><span class="sxs-lookup"><span data-stu-id="8b205-489">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="8b205-490">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="8b205-490">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="8b205-491">Atualização de Microsoft.Azure.Management.Storage 14.2.0 para suportar a nova versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8b205-491">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="8b205-492">Suporte de QuotaGiB (Quota de Partilha em Gibibye) para obter valores superiores a 5120 no plano de Gestão de cmdlets de Partilha de Ficheiros e foi adicionado o alias do parâmetro "Quota" ao parâmetro "QuotaGiB".</span><span class="sxs-lookup"><span data-stu-id="8b205-492">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="8b205-493">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-493">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="8b205-494">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-494">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="8b205-495">Adição do alias do parâmetro "QuotaGiB" ao parâmetro "Quota"</span><span class="sxs-lookup"><span data-stu-id="8b205-495">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="8b205-496">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="8b205-496">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="8b205-497">Correção do problema em que Set-AzStorageContainerAcl consegue limpar a Política de Acesso armazenada</span><span class="sxs-lookup"><span data-stu-id="8b205-497">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="8b205-498">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="8b205-498">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="8b205-499">3.1.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-499">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-500">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-500">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-501">Az.DataBoxEdge 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="8b205-501">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="8b205-502">Az.SqlVirtualMachine 1.0.0 já disponível</span><span class="sxs-lookup"><span data-stu-id="8b205-502">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-503">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-503">Az.Compute</span></span>
* <span data-ttu-id="8b205-504">Funcionalidade de Reaplicação da VM</span><span class="sxs-lookup"><span data-stu-id="8b205-504">VM Reapply feature</span></span>
    - <span data-ttu-id="8b205-505">Adição do parâmetro Reapply ao cmdlet Set-AzVM</span><span class="sxs-lookup"><span data-stu-id="8b205-505">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="8b205-506">Funcionalidade AutomaticRepairs do Conjunto de Dimensionamento de VM:</span><span class="sxs-lookup"><span data-stu-id="8b205-506">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="8b205-507">Adição dos parâmetros EnableAutomaticRepair, AutomaticRepairGracePeriod e AutomaticRepairMaxInstanceRepairsPercent aos seguintes cmdlets:   New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-507">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="8b205-508">Suporte para imagens de galeria entre inquilinos para New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8b205-508">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="8b205-509">Adição de "Spot" ao preenchedor de argumentos do parâmetro Priority nos cmdlets New-AzVM, New-AzVMConfig e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-509">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8b205-510">Adição dos parâmetros DiskIOPSReadWrite e DiskMBpsReadWrite ao cmdlet Add-AzVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="8b205-510">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="8b205-511">Alteração do parâmetro SourceImageId do cmdlet New-AzGalleryImageVersion para opcional</span><span class="sxs-lookup"><span data-stu-id="8b205-511">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="8b205-512">Adição dos parâmetros OSDiskImage e DataDiskImage ao cmdlet New-AzGalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="8b205-512">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="8b205-513">Adição do parâmetro HyperVGeneration ao cmdlet New-AzGalleryImageDefinition</span><span class="sxs-lookup"><span data-stu-id="8b205-513">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="8b205-514">Adição dos parâmetros SkipExtensionsOnOverprovisionedVMs aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-514">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="8b205-515">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="8b205-515">Az.DataBoxEdge</span></span>
* <span data-ttu-id="8b205-516">Adição do cmdlet `Get-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8b205-516">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8b205-517">Obter a Encomenda</span><span class="sxs-lookup"><span data-stu-id="8b205-517">Get the Order</span></span>
* <span data-ttu-id="8b205-518">Adição do cmdlet `New-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8b205-518">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8b205-519">Criar nova Encomenda</span><span class="sxs-lookup"><span data-stu-id="8b205-519">Create new Order</span></span>
* <span data-ttu-id="8b205-520">Adição do cmdlet `Remove-AzDataBoxEdgeOrder`</span><span class="sxs-lookup"><span data-stu-id="8b205-520">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="8b205-521">Remover a Encomenda</span><span class="sxs-lookup"><span data-stu-id="8b205-521">Remove the Order</span></span>
* <span data-ttu-id="8b205-522">Alteração no cmdlet `New-AzDataBoxEdgeShare`</span><span class="sxs-lookup"><span data-stu-id="8b205-522">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="8b205-523">Agora cria uma Partilha Local</span><span class="sxs-lookup"><span data-stu-id="8b205-523">Now creates Local Share</span></span>
* <span data-ttu-id="8b205-524">Adição do cmdlet `Set-AzDataBoxEdgeRole`</span><span class="sxs-lookup"><span data-stu-id="8b205-524">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="8b205-525">Agora, o IotRole pode ser mapeado para a Partilha</span><span class="sxs-lookup"><span data-stu-id="8b205-525">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="8b205-526">Adição do cmdlet `Invoke-AzDataBoxEdgeDevice`</span><span class="sxs-lookup"><span data-stu-id="8b205-526">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="8b205-527">Invocar verificação da atualização, transferência da atualização, instalação das atualizações no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b205-527">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="8b205-528">Adição do cmdlet `Get-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8b205-528">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8b205-529">Obtém as informações sobre os Acionadores</span><span class="sxs-lookup"><span data-stu-id="8b205-529">Gets the information about Triggers</span></span>
* <span data-ttu-id="8b205-530">Adição do cmdlet `New-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8b205-530">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8b205-531">Criar novos Acionadores</span><span class="sxs-lookup"><span data-stu-id="8b205-531">Create new Triggers</span></span>
* <span data-ttu-id="8b205-532">Adição do cmdlet `Remove-AzDataBoxEdgeTrigger`</span><span class="sxs-lookup"><span data-stu-id="8b205-532">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="8b205-533">Remover os Acionadores</span><span class="sxs-lookup"><span data-stu-id="8b205-533">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-534">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-534">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-535">Atualização do SDK .NET do ADF para a versão 4.4.0</span><span class="sxs-lookup"><span data-stu-id="8b205-535">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="8b205-536">Adição do parâmetro "ExpressCustomSetup" para o cmdlet "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir configurações e componentes de terceiros sem scripts de configuração personalizados.</span><span class="sxs-lookup"><span data-stu-id="8b205-536">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-537">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-537">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-538">Atualização da documentação de Get-AzDataLakeStoreDeletedItem e Restore-AzDataLakeStoreDeletedItem</span><span class="sxs-lookup"><span data-stu-id="8b205-538">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-539">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-539">Az.EventHub</span></span>
* <span data-ttu-id="8b205-540">Correção do problema 10301: Correção do formato de data do token de SAS</span><span class="sxs-lookup"><span data-stu-id="8b205-540">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-541">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-541">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-542">Adição do parâmetro MinimumTlsVersion a Enable-AzFrontDoorCustomDomainHttps e New-AzFrontDoorFrontendEndpointObject</span><span class="sxs-lookup"><span data-stu-id="8b205-542">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="8b205-543">Adição dos parâmetros HealthProbeMethod e EnabledState a New-AzFrontDoorHealthProbeSettingObject</span><span class="sxs-lookup"><span data-stu-id="8b205-543">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="8b205-544">Adição de um novo cmdlet para criar um objeto BackendPoolsSettings para passar para a criação/atualização do Front Door</span><span class="sxs-lookup"><span data-stu-id="8b205-544">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="8b205-545">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="8b205-545">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-546">Az.Network</span></span>
* <span data-ttu-id="8b205-547">Alteração dos exemplos de opções FilterData de "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" e "Start-AzVirtualnetworkGatewayPacketCapture.md".</span><span class="sxs-lookup"><span data-stu-id="8b205-547">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="8b205-548">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="8b205-548">Az.PrivateDns</span></span>
* <span data-ttu-id="8b205-549">Atualização do SDK .NET do PrivateDns para a versão 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8b205-549">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-550">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-550">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-551">Suporte do Azure Site Recovery para selecionar o tipo de disco ao ativar a proteção.</span><span class="sxs-lookup"><span data-stu-id="8b205-551">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="8b205-552">Correção do Azure Site Recovery para a edição de ações do plano de recuperação.</span><span class="sxs-lookup"><span data-stu-id="8b205-552">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="8b205-553">Suporte de Restauro de SQL do Azure Backup para aceitar BDs de filestream.</span><span class="sxs-lookup"><span data-stu-id="8b205-553">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8b205-554">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8b205-554">Az.RedisCache</span></span>
* <span data-ttu-id="8b205-555">Adição do parâmetro "MinimumTlsVersion" nos cmdlets "New-AzRedisCache" e "Set-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="8b205-555">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="8b205-556">Adição, também, de "MinimumTlsVersion" na saída do cmdlet "Get-AzRedisCache".</span><span class="sxs-lookup"><span data-stu-id="8b205-556">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="8b205-557">Adição da validação no parâmetro "-Size" para os cmdlets "Set-AzRedisCache" e "New-AzRedisCache"</span><span class="sxs-lookup"><span data-stu-id="8b205-557">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-558">Az.Resources</span></span>
- <span data-ttu-id="8b205-559">Atualização dos cmdlets de política no sentido de utilizar a nova versão de api 2019-06-01, a qual tem a nova propriedade EnforcementMode na atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="8b205-559">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="8b205-560">Atualização do exemplo de ajuda da definição da política de criação</span><span class="sxs-lookup"><span data-stu-id="8b205-560">Updated create policy definition help example</span></span>
- <span data-ttu-id="8b205-561">Correção do erro Remove-AZADServicePrincipal -ServicePrincipalName. Apresentação de uma referência nula quando o nome do principal do serviço não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="8b205-561">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="8b205-562">Correção do erro New-AZADServicePrincipal. Apresentação de uma referência nula quando o inquilino não tem uma subscrição.</span><span class="sxs-lookup"><span data-stu-id="8b205-562">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="8b205-563">Alteração de New-AzAdServicePrincipal para adicionar credenciais apenas a aplicações associadas.</span><span class="sxs-lookup"><span data-stu-id="8b205-563">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-564">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-564">Az.Sql</span></span>
* <span data-ttu-id="8b205-565">Adição de suporte para a base de dados ReadReplicaCount.</span><span class="sxs-lookup"><span data-stu-id="8b205-565">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="8b205-566">Correção de Set-AzSqlDatabase quando a redundância de zona não está definida</span><span class="sxs-lookup"><span data-stu-id="8b205-566">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="8b205-567">3.0.0 - Novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-567">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="8b205-568">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-568">General</span></span>
* <span data-ttu-id="8b205-569">Disponibilização do Az.PrivateDns 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8b205-569">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-570">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-570">Az.Accounts</span></span>
* <span data-ttu-id="8b205-571">Adição de uma mensagem de descontinuação para o alias "Resolve-Error".</span><span class="sxs-lookup"><span data-stu-id="8b205-571">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8b205-572">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8b205-572">Az.Advisor</span></span>
* <span data-ttu-id="8b205-573">Adição da nova categoria "Excelência Operacional" ao cmdlet Get-AzAdvisorRecommendation.</span><span class="sxs-lookup"><span data-stu-id="8b205-573">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8b205-574">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-574">Az.Batch</span></span>
* <span data-ttu-id="8b205-575">Mudança de nome de `CoreQuota` em `BatchAccountContext` para `DedicatedCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="8b205-575">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="8b205-576">Existe também um novo `LowPriorityCoreQuota`.</span><span class="sxs-lookup"><span data-stu-id="8b205-576">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="8b205-577">Isto afeta **Get-AzBatchAccount**.</span><span class="sxs-lookup"><span data-stu-id="8b205-577">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="8b205-578">O parâmetro **New-AzBatchTask** `-ResourceFile` assume agora uma coleção de objetos `PSResourceFile`, os quais podem ser construídos com o novo cmdlet **New-AzBatchResourceFile**.</span><span class="sxs-lookup"><span data-stu-id="8b205-578">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="8b205-579">Novo cmdlet **New-AzBatchResourceFile** para ajudar a criar objetos `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8b205-579">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="8b205-580">Estes podem ser fornecidos a **New-AzBatchTask** no parâmetro `-ResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8b205-580">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="8b205-581">Isto suporta dois novos tipos de ficheiro de recursos para além do caminho `HttpUrl` existente:</span><span class="sxs-lookup"><span data-stu-id="8b205-581">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="8b205-582">Os ficheiros de recursos baseados em `AutoStorageContainerName` transferem um contentor integral de armazenamento automático para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="8b205-582">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="8b205-583">Os ficheiros de recursos baseados em `StorageContainerUrl` transferem o contentor especificado no URL para o nó do Batch.</span><span class="sxs-lookup"><span data-stu-id="8b205-583">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="8b205-584">Remoção da propriedade `ApplicationPackages` de `PSApplication` devolvida por **Get-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="8b205-584">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8b205-585">Os pacotes específicos dentro de uma aplicação podem agora ser obtidos com **Get-AzBatchApplicationPackage**.</span><span class="sxs-lookup"><span data-stu-id="8b205-585">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="8b205-586">Por exemplo: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span><span class="sxs-lookup"><span data-stu-id="8b205-586">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="8b205-587">Mudança de nome de `ApplicationId` para `ApplicationName` em **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication** e **Set-AzBatchApplication**.</span><span class="sxs-lookup"><span data-stu-id="8b205-587">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="8b205-588">`ApplicationId` é agora um alias de `ApplicationName`.</span><span class="sxs-lookup"><span data-stu-id="8b205-588">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="8b205-589">Adição da nova propriedade `PSWindowsUserConfiguration` a `PSUserAccount`.</span><span class="sxs-lookup"><span data-stu-id="8b205-589">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="8b205-590">Mudança de nome de `Version` para `Name` em `PSApplicationPackage`.</span><span class="sxs-lookup"><span data-stu-id="8b205-590">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="8b205-591">Mudança de nome de `BlobSource` para `HttpUrl` em `PSResourceFile`.</span><span class="sxs-lookup"><span data-stu-id="8b205-591">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="8b205-592">Remoção da propriedade `OSDisk` de `PSVirtualMachineConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8b205-592">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="8b205-593">Remoção de **Set-AzBatchPoolOSVersion**.</span><span class="sxs-lookup"><span data-stu-id="8b205-593">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="8b205-594">Esta operação deixou de ser suportada.</span><span class="sxs-lookup"><span data-stu-id="8b205-594">This operation is no longer supported.</span></span>
* <span data-ttu-id="8b205-595">Remoção de `TargetOSVersion` de `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8b205-595">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8b205-596">Mudança de nome de `CurrentOSVersion` para `OSVersion` em `PSCloudServiceConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="8b205-596">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="8b205-597">Remoção de `DataEgressGiB` e `DataIngressGiB` de `PSPoolUsageMetrics`.</span><span class="sxs-lookup"><span data-stu-id="8b205-597">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="8b205-598">Remoção de **Get-AzBatchNodeAgentSku** e substituição deste por **Get-AzBatchSupportedImage**.</span><span class="sxs-lookup"><span data-stu-id="8b205-598">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="8b205-599">**Get-AzBatchSupportedImage** devolve os mesmos dados de **Get-AzBatchNodeAgentSku**, mas num formato mais acessível.</span><span class="sxs-lookup"><span data-stu-id="8b205-599">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="8b205-600">As novas imagens não verificadas agora também são devolvidas.</span><span class="sxs-lookup"><span data-stu-id="8b205-600">New non-verified images are also now returned.</span></span> <span data-ttu-id="8b205-601">Informações adicionais sobre `Capabilities` e `BatchSupportEndOfLife` para cada imagem também foram incluídas.</span><span class="sxs-lookup"><span data-stu-id="8b205-601">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="8b205-602">Adição da capacidade de montagem de sistemas de ficheiros remotos em cada nó de um conjunto através do novo parâmetro `MountConfiguration` de **New-AzBatchPool**.</span><span class="sxs-lookup"><span data-stu-id="8b205-602">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="8b205-603">Adição do suporte a regras de segurança de rede que bloqueiam o acesso de rede a um conjunto com base na porta de origem do tráfego.</span><span class="sxs-lookup"><span data-stu-id="8b205-603">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="8b205-604">Isto ocorre através da propriedade `SourcePortRanges` em `PSNetworkSecurityGroupRule`.</span><span class="sxs-lookup"><span data-stu-id="8b205-604">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="8b205-605">Ao executar um contentor, o Batch agora suporta a execução da tarefa no diretório de trabalho do contentor ou no diretório de trabalho da tarefa do Batch.</span><span class="sxs-lookup"><span data-stu-id="8b205-605">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="8b205-606">Isto é controlado pela propriedade `WorkingDirectory` em `PSTaskContainerSettings`.</span><span class="sxs-lookup"><span data-stu-id="8b205-606">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="8b205-607">Adição da capacidade de especificar uma coleção de IPs públicos em `PSNetworkConfiguration` através da nova propriedade `PublicIPs`.</span><span class="sxs-lookup"><span data-stu-id="8b205-607">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="8b205-608">Isto garante que os nós no Conjunto terão um IP da lista de IPs fornecidos pelo utilizador.</span><span class="sxs-lookup"><span data-stu-id="8b205-608">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="8b205-609">Quando não for especificado, o valor predefinido de `WaitForSuccess` em `PSSTartTask` é agora `$True` (era `$False`).</span><span class="sxs-lookup"><span data-stu-id="8b205-609">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="8b205-610">Quando não for especificado, o valor predefinido de `Scope` em `PSAutoUserSpecification` é agora `Pool` (era `Task` no Windows e `Pool` no Linux).</span><span class="sxs-lookup"><span data-stu-id="8b205-610">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-611">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-611">Az.Cdn</span></span>
* <span data-ttu-id="8b205-612">Introdução de UrlRewriteAction e CacheKeyQueryStringAction em RulesEngine.</span><span class="sxs-lookup"><span data-stu-id="8b205-612">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="8b205-613">Correção de vários erros como a falta da Entrada "Seletor" no cmdlet New-AzDeliveryRuleCondition.</span><span class="sxs-lookup"><span data-stu-id="8b205-613">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-614">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-614">Az.Compute</span></span>
* <span data-ttu-id="8b205-615">Funcionalidade Conjunto de Encriptação de Discos</span><span class="sxs-lookup"><span data-stu-id="8b205-615">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="8b205-616">Novos cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="8b205-616">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="8b205-617">Adição do parâmetro DiskEncryptionSetId aos seguintes cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="8b205-617">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="8b205-618">Adição dos parâmetros DiskEncryptionSetId e EncryptionType aos seguintes cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-618">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8b205-619">Adição do parâmetro PublicIPAddressVersion a New-AzVmssIPConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-619">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="8b205-620">Movimentação de FileUris da extensão de script personalizado da definição pública para a definição protegida</span><span class="sxs-lookup"><span data-stu-id="8b205-620">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="8b205-621">Adição de ScaleInPolicy aos cmdlets New-AzVmss, New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-621">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="8b205-622">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8b205-622">Breaking changes</span></span>
    - <span data-ttu-id="8b205-623">Utilização do parâmetro UploadSizeInBytes em vez de DiskSizeGB para New-AzDiskConfig quando CreateOption é Carregar</span><span class="sxs-lookup"><span data-stu-id="8b205-623">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="8b205-624">Substituição de PublishingProfile.Source.ManagedImage.Id por StorageProfile.Source.Id no objeto GalleryImageVersion</span><span class="sxs-lookup"><span data-stu-id="8b205-624">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-625">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-625">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-626">Atualização da versão do SDK .Net do ADF para 4.3.0</span><span class="sxs-lookup"><span data-stu-id="8b205-626">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-627">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-627">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-628">Atualização da versão do SDK ADLS (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) ) com as seguintes correções</span><span class="sxs-lookup"><span data-stu-id="8b205-628">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="8b205-629">Evita a apresentação de uma exceção ao mesmo tempo que não consegue anular a serialização do creationtime do lixo ou da entrada de diretório.</span><span class="sxs-lookup"><span data-stu-id="8b205-629">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="8b205-630">Expõe a definição por tempo limite do pedido em adlsclient</span><span class="sxs-lookup"><span data-stu-id="8b205-630">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="8b205-631">Correção da passagem do syncflag original para a recuperação de badoffset</span><span class="sxs-lookup"><span data-stu-id="8b205-631">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="8b205-632">Correção de EnumerateDirectory para obter o token de continuação após a verificação da resposta</span><span class="sxs-lookup"><span data-stu-id="8b205-632">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="8b205-633">Correção do Erro de Concatenação</span><span class="sxs-lookup"><span data-stu-id="8b205-633">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-634">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-634">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-635">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="8b205-635">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-636">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-636">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-637">Correção do erro em que o cliente recebe o erro "Não é uma cadeia Base 64 válida" quando utiliza Get-AzHDInsightCluster para obter o cluster com o armazenamento ADLSGen1.</span><span class="sxs-lookup"><span data-stu-id="8b205-637">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="8b205-638">Adição de um parâmetro com o nome "ApplicationId" a três cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig e New-AzHDInsightCluster para que o cliente consiga fornecer o ID da aplicação do principal de serviço que permite aceder ao Azure Data Lake.</span><span class="sxs-lookup"><span data-stu-id="8b205-638">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="8b205-639">Alteração de Microsoft.Azure.Management.HDInsight da versão 2.1.0 para a 5.1.0</span><span class="sxs-lookup"><span data-stu-id="8b205-639">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="8b205-640">Remoção de cinco cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-640">Removed five cmdlets:</span></span>
    - <span data-ttu-id="8b205-641">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8b205-641">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8b205-642">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8b205-642">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8b205-643">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="8b205-643">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="8b205-644">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8b205-644">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="8b205-645">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8b205-645">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="8b205-646">Adição de três cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-646">Added three cmdlets:</span></span>
    - <span data-ttu-id="8b205-647">Get-AzHDInsightMonitoring para substituir Get-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8b205-647">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8b205-648">Enable-AzHDInsightMonitoring para substituir Enable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8b205-648">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="8b205-649">Disable-AzHDInsightMonitoring para substituir Disable-AzHDInsightOMS.</span><span class="sxs-lookup"><span data-stu-id="8b205-649">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="8b205-650">Correção do cmdlet Get-AzHDInsightProperties para suportar a obtenção de informações sobre capacidades de uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="8b205-650">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="8b205-651">Remoção de conjuntos de parâmetros("Spark1", "Spark2") de Add-AzHDInsightConfigValue.</span><span class="sxs-lookup"><span data-stu-id="8b205-651">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="8b205-652">Adição de exemplos aos documentos de ajuda do cmdlet Add-AzHDInsightSecurityProfile.</span><span class="sxs-lookup"><span data-stu-id="8b205-652">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="8b205-653">Alteração do tipo de saída dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-653">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="8b205-654">Alteração do tipo de saída de Get-AzHDInsightProperties de CapabilitiesResponse para AzureHDInsightCapabilities.</span><span class="sxs-lookup"><span data-stu-id="8b205-654">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="8b205-655">Alteração do tipo de saída de Remove-AzHDInsightCluster de ClusterGetResponse para booleano.</span><span class="sxs-lookup"><span data-stu-id="8b205-655">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="8b205-656">Alteração do tipo de saída de Set-AzHDInsightGatewaySettings de HttpConnectivitySettings para GatewaySettings.</span><span class="sxs-lookup"><span data-stu-id="8b205-656">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="8b205-657">Adição de alguns casos de teste de cenários.</span><span class="sxs-lookup"><span data-stu-id="8b205-657">Added some scenario test cases.</span></span>
* <span data-ttu-id="8b205-658">Remoção de alguns alias: "Add-AzHDInsightConfigValues", "Get-AzHDInsightProperties".</span><span class="sxs-lookup"><span data-stu-id="8b205-658">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-659">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-659">Az.IotHub</span></span>
* <span data-ttu-id="8b205-660">Alterações interruptivas:</span><span class="sxs-lookup"><span data-stu-id="8b205-660">Breaking changes:</span></span>
    - <span data-ttu-id="8b205-661">O cmdlet "Add-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8b205-661">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8b205-662">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Add-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8b205-662">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8b205-663">O cmdlet "Get-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8b205-663">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8b205-664">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Get-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8b205-664">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8b205-665">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="8b205-665">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="8b205-666">A propriedade "OperationsMonitoringProperties" do tipo "Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties" foi removida.</span><span class="sxs-lookup"><span data-stu-id="8b205-666">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="8b205-667">O cmdlet "New-AzIotHubExportDevice" deixou de suportar o alias "New-AzIotHubExportDevices".</span><span class="sxs-lookup"><span data-stu-id="8b205-667">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="8b205-668">O cmdlet "New-AzIotHubImportDevice" deixou de suportar o alias "New-AzIotHubImportDevices".</span><span class="sxs-lookup"><span data-stu-id="8b205-668">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="8b205-669">O cmdlet "Remove-AzIotHubEventHubConsumerGroup" deixou de suportar o parâmetro "EventHubEndpointName" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8b205-669">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8b205-670">O conjunto de parâmetros "__AllParameterSets" do cmdlet "Remove-AzIotHubEventHubConsumerGroup" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8b205-670">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="8b205-671">O cmdlet "Set-AzIotHub" deixou de suportar o parâmetro "OperationsMonitoringProperties" e não foi encontrado qualquer alias para o nome de parâmetro original.</span><span class="sxs-lookup"><span data-stu-id="8b205-671">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="8b205-672">O conjunto de parâmetros "UpdateOperationsMonitoringProperties" do cmdlet "Set-AzIotHub" foi removido.</span><span class="sxs-lookup"><span data-stu-id="8b205-672">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-673">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-673">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-674">Suporte do Azure Site Recovery para configurar recursos de rede como NSG, IP público e balanceadores de carga internos do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-674">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-675">Suporte do Azure Site Recovery para escrever para um disco gerido do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-675">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="8b205-676">Suporte do Azure Site Recovery para redução de NIC do VMware para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-676">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="8b205-677">Suporte do Azure Site Recovery para aceleração de rede do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-677">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-678">Suporte do Azure Site Recovery para a atualização automática do agente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-678">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-679">Suporte do Azure Site Recovery para SSD Standard do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-679">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-680">Suporte do Azure Site Recovery para a codificação em dois passos do Azure Disk Encryption do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-680">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-681">Suporte do Azure Site Recovery para a proteção de um disco adicionado recentemente do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-681">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-682">Adição da funcionalidade SoftDelete para VM e de testes para softdelete</span><span class="sxs-lookup"><span data-stu-id="8b205-682">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-683">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-683">Az.Resources</span></span>
* <span data-ttu-id="8b205-684">Atualização da assemblagem de dependências Microsoft.Extensions.Caching.Memory da versão 1.1.1 para a 2.2</span><span class="sxs-lookup"><span data-stu-id="8b205-684">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-685">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-685">Az.Network</span></span>
* <span data-ttu-id="8b205-686">Alteração de todos os cmdlets para PrivateEndpointConnection para suportar o fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="8b205-686">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="8b205-687">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-687">Updated cmdlet:</span></span>
        - <span data-ttu-id="8b205-688">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-688">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-689">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-689">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-690">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-690">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-691">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-691">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-692">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-692">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8b205-693">Adição de novo cmdlet para PrivateLinkResource também com suporte de fornecedor de serviços genérico.</span><span class="sxs-lookup"><span data-stu-id="8b205-693">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="8b205-694">Novo cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8b205-694">New cmdlet:</span></span>
        - <span data-ttu-id="8b205-695">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="8b205-695">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="8b205-696">Adição de novos campos e parâmetro para a funcionalidade Protocolo de Proxy V2.</span><span class="sxs-lookup"><span data-stu-id="8b205-696">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="8b205-697">Adição da propriedade EnableProxyProtocol em PrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-697">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="8b205-698">Adição da propriedade LinkIdentifier em PrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-698">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="8b205-699">Atualização de New-AzPrivateLinkService para adicionar um novo parâmetro adicional EnableProxyProtocol.</span><span class="sxs-lookup"><span data-stu-id="8b205-699">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="8b205-700">Correção da descrição incorreta do parâmetro na documentação de referência "New-AzApplicationGatewaySku"</span><span class="sxs-lookup"><span data-stu-id="8b205-700">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="8b205-701">Novos cmdlets para suportar a política de firewall do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-701">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="8b205-702">Adição de suporte para o recurso subordinado RouteTables de VirtualHub</span><span class="sxs-lookup"><span data-stu-id="8b205-702">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="8b205-703">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-703">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-704">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="8b205-704">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="8b205-705">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-705">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8b205-706">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-706">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8b205-707">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-707">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="8b205-708">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="8b205-708">Set-AzVirtualHub</span></span>
* <span data-ttu-id="8b205-709">Adição de suporte para o SKU de novas propriedades de VirtualHub e VirtualWANType de VirtualWan</span><span class="sxs-lookup"><span data-stu-id="8b205-709">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="8b205-710">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8b205-710">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8b205-711">New-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="8b205-711">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8b205-712">Update-AzVirtualHub : adição do parâmetro Sku</span><span class="sxs-lookup"><span data-stu-id="8b205-712">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="8b205-713">New-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="8b205-713">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="8b205-714">Update-AzVirtualWan : adição do parâmetro VirtualWANType</span><span class="sxs-lookup"><span data-stu-id="8b205-714">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="8b205-715">Adição de suporte para a propriedade EnableInternetSecurity para HubVnetConnection, VpnConnection e ExpressRouteConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-715">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="8b205-716">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-716">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-717">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-717">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="8b205-718">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8b205-718">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8b205-719">New-AzureRmVirtualHubVnetConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8b205-719">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8b205-720">New-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8b205-720">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8b205-721">Update-AzureRmVpnConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8b205-721">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8b205-722">New-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8b205-722">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="8b205-723">Set-AzureRmExpressRouteConnection : adição do parâmetro EnableInternetSecurity</span><span class="sxs-lookup"><span data-stu-id="8b205-723">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="8b205-724">Adição de suporte para Configurar a Política WebApplicationFirewall de Nível Superior</span><span class="sxs-lookup"><span data-stu-id="8b205-724">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="8b205-725">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-725">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-726">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="8b205-726">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="8b205-727">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="8b205-727">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="8b205-728">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="8b205-728">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="8b205-729">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="8b205-729">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="8b205-730">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="8b205-730">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="8b205-731">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-731">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="8b205-732">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8b205-732">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8b205-733">New-AzApplicationGatewayFirewallPolicy : adição do parâmetro PolicySetting, ManagedRule</span><span class="sxs-lookup"><span data-stu-id="8b205-733">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="8b205-734">Adição de suporte para o operador GeoMatch em CustomRule</span><span class="sxs-lookup"><span data-stu-id="8b205-734">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="8b205-735">Adição de GeoMatch ao operador em FirewallCondition</span><span class="sxs-lookup"><span data-stu-id="8b205-735">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="8b205-736">Adição de suporte para a Política de firewall perListener e perSite</span><span class="sxs-lookup"><span data-stu-id="8b205-736">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="8b205-737">Cmdlets atualizados com parâmetros adicionais:</span><span class="sxs-lookup"><span data-stu-id="8b205-737">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="8b205-738">New-AzApplicationGatewayHttpListener : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="8b205-738">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="8b205-739">New-AzApplicationGatewayPathRuleConfig : adição do parâmetro FirewallPolicy, FirewallPolicyId</span><span class="sxs-lookup"><span data-stu-id="8b205-739">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="8b205-740">Correção da sub-rede necessária com o nome AzureBastionSubnet em "PSBastion" pode não ser sensível às maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="8b205-740">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="8b205-741">Suporte para FQDNs de Destino nas Regras de Rede e para FQDN Traduzido em Regras NAT para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8b205-741">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="8b205-742">Adição de suporte para o recurso de nível superior RouteTables de IpGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-742">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="8b205-743">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-743">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-744">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-744">New-AzIpGroup</span></span>
        - <span data-ttu-id="8b205-745">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-745">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="8b205-746">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-746">Get-AzIpGroup</span></span>
        - <span data-ttu-id="8b205-747">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-747">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-748">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-748">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-749">Remoção do cmdlet Add-AzServiceFabricApplicationCertificate uma vez que este cenário é abrangido por Add-AzVmssSecret.</span><span class="sxs-lookup"><span data-stu-id="8b205-749">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-750">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-750">Az.Sql</span></span>
* <span data-ttu-id="8b205-751">Adição de suporte para o restauro de bases de dados removidas em Instâncias Geridas.</span><span class="sxs-lookup"><span data-stu-id="8b205-751">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="8b205-752">Descontinuação dos cmdlets de auditoria antigos do código.</span><span class="sxs-lookup"><span data-stu-id="8b205-752">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="8b205-753">Remoção de aliases descontinuados:</span><span class="sxs-lookup"><span data-stu-id="8b205-753">Removed deprecated aliases:</span></span>
* <span data-ttu-id="8b205-754">Get-AzSqlDatabaseIndexRecommendations (utilize antes Get-AzSqlDatabaseIndexRecommendation)</span><span class="sxs-lookup"><span data-stu-id="8b205-754">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="8b205-755">Get-AzSqlDatabaseRestorePoints (utilize antes Get-AzSqlDatabaseRestorePoint)</span><span class="sxs-lookup"><span data-stu-id="8b205-755">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="8b205-756">Remoção do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-756">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8b205-757">Remoção dos aliases dos cmdlets descontinuados das Definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="8b205-757">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="8b205-758">Descontinuação dos cmdlets das Definições de Deteção Avançada de Ameaças</span><span class="sxs-lookup"><span data-stu-id="8b205-758">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="8b205-759">Adição de cmdlets para Desativar e Ativar as recomendações de sensibilidade nas colunas de uma base de dados.</span><span class="sxs-lookup"><span data-stu-id="8b205-759">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-760">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-760">Az.Storage</span></span>
* <span data-ttu-id="8b205-761">Suporte à ativação da partilha de Ficheiros de Grandes Dimensões ao criar ou atualizar uma Conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b205-761">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="8b205-762">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-762">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8b205-763">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-763">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8b205-764">Ao fechar/obter o Identificador de ficheiro, ignorar a verificação do caminho de entrada corresponde a Diretório de ficheiros ou Ficheiro, de forma a evitar a falha com o objeto no estado DeletePending</span><span class="sxs-lookup"><span data-stu-id="8b205-764">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="8b205-765">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8b205-765">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="8b205-766">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8b205-766">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="8b205-767">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-767">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="8b205-768">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-768">General</span></span>
* <span data-ttu-id="8b205-769">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8b205-769">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-770">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-770">Az.Accounts</span></span>
* <span data-ttu-id="8b205-771">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="8b205-771">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8b205-772">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-772">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-773">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="8b205-773">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="8b205-774">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="8b205-774">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-775">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-775">Az.Automation</span></span>
* <span data-ttu-id="8b205-776">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="8b205-776">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8b205-777">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-777">Az.Batch</span></span>
* <span data-ttu-id="8b205-778">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="8b205-778">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-779">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-779">Az.Compute</span></span>
* <span data-ttu-id="8b205-780">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-780">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="8b205-781">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="8b205-781">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="8b205-782">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="8b205-782">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="8b205-783">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="8b205-783">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-784">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-784">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-785">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="8b205-785">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="8b205-786">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="8b205-786">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="8b205-787">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="8b205-787">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-788">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-788">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-789">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="8b205-789">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="8b205-790">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="8b205-790">Az.HealthcareApis</span></span>
* <span data-ttu-id="8b205-791">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="8b205-791">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="8b205-792">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="8b205-792">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="8b205-793">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="8b205-793">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="8b205-794">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="8b205-794">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-795">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-795">Az.IotHub</span></span>
* <span data-ttu-id="8b205-796">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="8b205-796">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="8b205-797">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="8b205-797">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-798">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-798">Az.Monitor</span></span>
* <span data-ttu-id="8b205-799">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="8b205-799">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="8b205-800">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="8b205-800">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="8b205-801">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="8b205-801">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="8b205-802">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8b205-802">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-803">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-803">Az.Network</span></span>
* <span data-ttu-id="8b205-804">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="8b205-804">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="8b205-805">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8b205-805">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="8b205-806">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-806">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-807">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-807">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="8b205-808">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-808">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8b205-809">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="8b205-809">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="8b205-810">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="8b205-810">Updated cmdlets:</span></span>
        - <span data-ttu-id="8b205-811">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-811">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8b205-812">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-812">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8b205-813">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-813">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8b205-814">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="8b205-814">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="8b205-815">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="8b205-815">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="8b205-816">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="8b205-816">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="8b205-817">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="8b205-817">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8b205-818">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8b205-818">Az.RedisCache</span></span>
* <span data-ttu-id="8b205-819">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="8b205-819">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-820">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-820">Az.Sql</span></span>
* <span data-ttu-id="8b205-821">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="8b205-821">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-822">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-822">Az.Storage</span></span>
* <span data-ttu-id="8b205-823">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="8b205-823">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="8b205-824">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="8b205-824">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8b205-825">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="8b205-825">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="8b205-826">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="8b205-826">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="8b205-827">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-827">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8b205-828">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8b205-828">Az.StorageSync</span></span>
* <span data-ttu-id="8b205-829">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="8b205-829">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-830">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-830">Az.Websites</span></span>
* <span data-ttu-id="8b205-831">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="8b205-831">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="8b205-832">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-832">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8b205-833">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-833">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-834">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="8b205-834">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="8b205-835">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="8b205-835">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="8b205-836">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="8b205-836">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-837">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-837">Az.Automation</span></span>
* <span data-ttu-id="8b205-838">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="8b205-838">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="8b205-839">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="8b205-839">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="8b205-840">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="8b205-840">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-841">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-841">Az.Compute</span></span>
* <span data-ttu-id="8b205-842">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-842">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="8b205-843">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-843">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8b205-844">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="8b205-844">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="8b205-845">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="8b205-845">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="8b205-846">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="8b205-846">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="8b205-847">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="8b205-847">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="8b205-848">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="8b205-848">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="8b205-849">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="8b205-849">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="8b205-850">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="8b205-850">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-851">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-851">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-852">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="8b205-852">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="8b205-853">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="8b205-853">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-854">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-854">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-855">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8b205-855">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-856">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-856">Az.IotHub</span></span>
* <span data-ttu-id="8b205-857">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="8b205-857">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="8b205-858">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="8b205-858">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="8b205-859">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="8b205-859">New cmdlets are:</span></span>
    - <span data-ttu-id="8b205-860">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8b205-860">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8b205-861">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8b205-861">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8b205-862">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8b205-862">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="8b205-863">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="8b205-863">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-864">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-864">Az.Monitor</span></span>
* <span data-ttu-id="8b205-865">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="8b205-865">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="8b205-866">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="8b205-866">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="8b205-867">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8b205-867">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="8b205-868">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="8b205-868">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="8b205-869">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="8b205-869">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="8b205-870">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="8b205-870">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="8b205-871">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8b205-871">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="8b205-872">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="8b205-872">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="8b205-873">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="8b205-873">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8b205-874">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="8b205-874">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="8b205-875">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="8b205-875">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="8b205-876">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="8b205-876">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="8b205-877">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="8b205-877">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="8b205-878">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="8b205-878">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="8b205-879">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="8b205-879">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="8b205-880">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="8b205-880">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="8b205-881">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="8b205-881">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="8b205-882">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-882">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="8b205-883">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="8b205-883">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="8b205-884">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-884">Overall improved help files</span></span>
* <span data-ttu-id="8b205-885">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="8b205-885">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-886">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-886">Az.Network</span></span>
* <span data-ttu-id="8b205-887">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="8b205-887">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="8b205-888">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="8b205-888">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="8b205-889">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="8b205-889">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="8b205-890">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="8b205-890">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="8b205-891">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="8b205-891">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="8b205-892">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="8b205-892">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="8b205-893">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="8b205-893">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="8b205-894">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="8b205-894">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="8b205-895">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-895">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="8b205-896">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="8b205-896">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="8b205-897">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8b205-897">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="8b205-898">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="8b205-898">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="8b205-899">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-899">New cmdlets</span></span>
        - <span data-ttu-id="8b205-900">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="8b205-900">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="8b205-901">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-901">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="8b205-902">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-902">Updated cmdlet:</span></span>
        - <span data-ttu-id="8b205-903">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8b205-903">New-VpnSite</span></span>
        - <span data-ttu-id="8b205-904">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="8b205-904">Update-VpnSite</span></span>
        - <span data-ttu-id="8b205-905">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-905">New-VpnConnection</span></span>
        - <span data-ttu-id="8b205-906">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-906">Update-VpnConnection</span></span>
* <span data-ttu-id="8b205-907">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="8b205-907">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-908">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-908">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-909">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="8b205-909">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="8b205-910">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="8b205-910">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-911">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-911">Az.Resources</span></span>
* <span data-ttu-id="8b205-912">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="8b205-912">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-913">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-913">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-914">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="8b205-914">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="8b205-915">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="8b205-915">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="8b205-916">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8b205-916">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8b205-917">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8b205-917">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8b205-918">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8b205-918">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8b205-919">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8b205-919">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="8b205-920">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8b205-920">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8b205-921">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8b205-921">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8b205-922">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8b205-922">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8b205-923">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8b205-923">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8b205-924">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="8b205-924">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="8b205-925">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="8b205-925">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="8b205-926">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="8b205-926">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="8b205-927">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8b205-927">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="8b205-928">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="8b205-928">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="8b205-929">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="8b205-929">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8b205-930">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8b205-930">Az.SignalR</span></span>
* <span data-ttu-id="8b205-931">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="8b205-931">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-932">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-932">Az.Sql</span></span>
* <span data-ttu-id="8b205-933">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="8b205-933">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="8b205-934">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="8b205-934">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="8b205-935">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-935">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="8b205-936">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8b205-936">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="8b205-937">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="8b205-937">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-938">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-938">Az.Storage</span></span>
* <span data-ttu-id="8b205-939">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="8b205-939">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="8b205-940">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="8b205-940">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="8b205-941">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8b205-941">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="8b205-942">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8b205-942">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="8b205-943">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="8b205-943">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="8b205-944">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8b205-944">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="8b205-945">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="8b205-945">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="8b205-946">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-946">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8b205-947">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-947">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8b205-948">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-948">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="8b205-949">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="8b205-949">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-950">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-950">Az.Websites</span></span>
* <span data-ttu-id="8b205-951">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="8b205-951">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="8b205-952">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="8b205-952">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="8b205-953">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="8b205-953">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="8b205-954">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-954">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="8b205-955">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-955">General</span></span>
* <span data-ttu-id="8b205-956">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="8b205-956">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-957">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-957">Az.Accounts</span></span>
* <span data-ttu-id="8b205-958">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="8b205-958">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="8b205-959">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8b205-959">Az.Aks</span></span>
* <span data-ttu-id="8b205-960">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="8b205-960">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="8b205-961">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="8b205-961">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8b205-962">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-962">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-963">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="8b205-963">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="8b205-964">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="8b205-964">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="8b205-965">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="8b205-965">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="8b205-966">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="8b205-966">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="8b205-967">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="8b205-967">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8b205-968">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-968">Az.Batch</span></span>
* <span data-ttu-id="8b205-969">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="8b205-969">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-970">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-970">Az.Cdn</span></span>
* <span data-ttu-id="8b205-971">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="8b205-971">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-972">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-972">Az.Compute</span></span>
* <span data-ttu-id="8b205-973">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-973">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="8b205-974">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-974">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="8b205-975">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="8b205-975">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="8b205-976">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="8b205-976">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="8b205-977">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="8b205-977">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="8b205-978">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8b205-978">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="8b205-979">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="8b205-979">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="8b205-980">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="8b205-980">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-981">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-981">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-982">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="8b205-982">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="8b205-983">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="8b205-983">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="8b205-984">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="8b205-984">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="8b205-985">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="8b205-985">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-986">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-986">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-987">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="8b205-987">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-988">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-988">Az.EventHub</span></span>
* <span data-ttu-id="8b205-989">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-989">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="8b205-990">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="8b205-990">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="8b205-991">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="8b205-991">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="8b205-992">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="8b205-992">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="8b205-993">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8b205-993">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8b205-994">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="8b205-994">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-995">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-995">Az.Monitor</span></span>
* <span data-ttu-id="8b205-996">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-996">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-997">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-997">Az.Network</span></span>
* <span data-ttu-id="8b205-998">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="8b205-998">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="8b205-999">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="8b205-999">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="8b205-1000">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="8b205-1000">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="8b205-1001">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="8b205-1001">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="8b205-1002">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="8b205-1002">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="8b205-1003">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8b205-1003">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="8b205-1004">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="8b205-1004">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1005">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1005">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1006">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="8b205-1006">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="8b205-1007">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="8b205-1007">Added example</span></span>
    - <span data-ttu-id="8b205-1008">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="8b205-1008">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="8b205-1009">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="8b205-1009">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="8b205-1010">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="8b205-1010">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1011">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1011">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1012">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1012">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1013">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1013">Az.Resources</span></span>
* <span data-ttu-id="8b205-1014">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="8b205-1014">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="8b205-1015">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="8b205-1015">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="8b205-1016">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="8b205-1016">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="8b205-1017">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-1017">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-1018">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-1018">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-1019">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1019">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="8b205-1020">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="8b205-1020">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="8b205-1021">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="8b205-1021">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-1022">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1022">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-1023">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="8b205-1023">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="8b205-1024">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="8b205-1024">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="8b205-1025">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="8b205-1025">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="8b205-1026">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="8b205-1026">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="8b205-1027">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="8b205-1027">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="8b205-1028">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="8b205-1028">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1029">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1029">Az.Sql</span></span>
* <span data-ttu-id="8b205-1030">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="8b205-1030">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1031">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1031">Az.Storage</span></span>
* <span data-ttu-id="8b205-1032">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="8b205-1032">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="8b205-1033">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="8b205-1033">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="8b205-1034">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8b205-1034">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="8b205-1035">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-1035">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="8b205-1036">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="8b205-1036">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="8b205-1037">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-1037">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1038">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1038">Az.Websites</span></span>
* <span data-ttu-id="8b205-1039">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8b205-1039">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="8b205-1040">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1040">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1041">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1041">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1042">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8b205-1042">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8b205-1043">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1043">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8b205-1044">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="8b205-1044">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1045">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1045">Az.Automation</span></span>
* <span data-ttu-id="8b205-1046">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="8b205-1046">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-1047">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1047">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-1048">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="8b205-1048">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1049">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1049">Az.Compute</span></span>
* <span data-ttu-id="8b205-1050">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="8b205-1050">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8b205-1051">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8b205-1051">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8b205-1052">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="8b205-1052">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="8b205-1053">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="8b205-1053">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1054">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1054">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1055">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8b205-1055">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="8b205-1056">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="8b205-1056">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-1057">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1057">Az.EventHub</span></span>
* <span data-ttu-id="8b205-1058">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8b205-1058">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8b205-1059">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="8b205-1059">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-1060">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1060">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-1061">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="8b205-1061">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8b205-1062">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1062">Az.LogicApp</span></span>
* <span data-ttu-id="8b205-1063">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="8b205-1063">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="8b205-1064">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="8b205-1064">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="8b205-1065">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1065">Az.ManagedServices</span></span>
* <span data-ttu-id="8b205-1066">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="8b205-1066">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1067">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1067">Az.Network</span></span>
* <span data-ttu-id="8b205-1068">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="8b205-1068">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="8b205-1069">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1069">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1070">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-1070">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8b205-1071">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1071">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8b205-1072">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1072">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-1073">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1073">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-1074">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1074">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-1075">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1075">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8b205-1076">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="8b205-1076">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="8b205-1077">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1077">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="8b205-1078">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="8b205-1078">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="8b205-1079">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1079">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="8b205-1080">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8b205-1080">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="8b205-1081">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="8b205-1081">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="8b205-1082">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="8b205-1082">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="8b205-1083">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="8b205-1083">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="8b205-1084">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="8b205-1084">Updated cmdlets</span></span>
        - <span data-ttu-id="8b205-1085">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1085">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8b205-1086">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1086">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8b205-1087">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1087">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8b205-1088">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1088">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8b205-1089">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1089">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="8b205-1090">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-1090">Updated cmdlet:</span></span>
        - <span data-ttu-id="8b205-1091">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1091">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8b205-1092">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1092">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8b205-1093">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1093">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="8b205-1094">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="8b205-1094">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="8b205-1095">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="8b205-1095">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="8b205-1096">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="8b205-1096">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1097">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1097">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1098">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="8b205-1098">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="8b205-1099">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="8b205-1099">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1100">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1100">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1101">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1101">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8b205-1102">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1102">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="8b205-1103">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1103">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="8b205-1104">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1104">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8b205-1105">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1105">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="8b205-1106">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1106">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8b205-1107">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1107">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="8b205-1108">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1108">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8b205-1109">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1109">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="8b205-1110">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="8b205-1110">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1111">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1111">Az.Resources</span></span>
- <span data-ttu-id="8b205-1112">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8b205-1112">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="8b205-1113">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="8b205-1113">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-1114">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-1114">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-1115">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8b205-1115">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8b205-1116">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="8b205-1116">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1117">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1117">Az.Sql</span></span>
* <span data-ttu-id="8b205-1118">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="8b205-1118">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="8b205-1119">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="8b205-1119">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="8b205-1120">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="8b205-1120">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1121">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1121">Az.Storage</span></span>
* <span data-ttu-id="8b205-1122">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="8b205-1122">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8b205-1123">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8b205-1123">Az.StorageSync</span></span>
* <span data-ttu-id="8b205-1124">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="8b205-1124">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="8b205-1125">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="8b205-1125">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1126">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1126">Az.Websites</span></span>
* <span data-ttu-id="8b205-1127">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1127">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="8b205-1128">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1128">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="8b205-1129">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1129">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="8b205-1130">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1130">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1131">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1131">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1132">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="8b205-1132">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8b205-1133">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="8b205-1133">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8b205-1134">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="8b205-1134">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8b205-1135">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8b205-1135">Az.Advisor</span></span>
* <span data-ttu-id="8b205-1136">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8b205-1136">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8b205-1137">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="8b205-1137">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8b205-1138">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-1138">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-1139">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8b205-1139">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8b205-1140">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8b205-1140">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8b205-1141">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="8b205-1141">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8b205-1142">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="8b205-1142">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8b205-1143">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="8b205-1143">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8b205-1144">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8b205-1144">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8b205-1145">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="8b205-1145">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1146">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1146">Az.Automation</span></span>
* <span data-ttu-id="8b205-1147">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="8b205-1147">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1148">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1148">Az.Compute</span></span>
* <span data-ttu-id="8b205-1149">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1149">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1150">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1150">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1151">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="8b205-1151">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8b205-1152">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8b205-1152">Az.EventGrid</span></span>
* <span data-ttu-id="8b205-1153">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="8b205-1153">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-1154">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1154">Az.IotHub</span></span>
* <span data-ttu-id="8b205-1155">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="8b205-1155">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1156">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1156">Az.Network</span></span>
* <span data-ttu-id="8b205-1157">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="8b205-1157">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8b205-1158">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="8b205-1158">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-1159">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1159">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-1160">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="8b205-1160">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8b205-1161">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8b205-1161">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1162">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1162">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1163">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="8b205-1163">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1164">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1165">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="8b205-1165">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1166">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1166">Az.Resources</span></span>
    - <span data-ttu-id="8b205-1167">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="8b205-1167">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8b205-1168">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="8b205-1168">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8b205-1169">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="8b205-1169">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8b205-1170">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="8b205-1170">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-1171">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-1171">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-1172">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="8b205-1172">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1173">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1173">Az.Sql</span></span>
* <span data-ttu-id="8b205-1174">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="8b205-1174">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8b205-1175">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1175">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8b205-1176">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1176">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8b205-1177">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1177">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8b205-1178">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1178">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8b205-1179">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1179">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8b205-1180">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1180">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8b205-1181">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8b205-1181">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8b205-1182">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="8b205-1182">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1183">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1183">Az.Storage</span></span>
* <span data-ttu-id="8b205-1184">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="8b205-1184">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8b205-1185">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8b205-1185">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8b205-1186">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="8b205-1186">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8b205-1187">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="8b205-1187">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8b205-1188">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1188">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8b205-1189">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1189">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8b205-1190">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1190">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8b205-1191">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="8b205-1191">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8b205-1192">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8b205-1192">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8b205-1193">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8b205-1193">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8b205-1194">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8b205-1194">Az.StorageSync</span></span>
* <span data-ttu-id="8b205-1195">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="8b205-1195">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8b205-1196">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1196">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1197">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1197">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1198">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="8b205-1198">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8b205-1199">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8b205-1199">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8b205-1200">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8b205-1200">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8b205-1201">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8b205-1201">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8b205-1202">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8b205-1202">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1203">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1203">Az.Compute</span></span>
* <span data-ttu-id="8b205-1204">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="8b205-1204">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8b205-1205">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="8b205-1205">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8b205-1206">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8b205-1206">Az.Dns</span></span>
* <span data-ttu-id="8b205-1207">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="8b205-1207">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8b205-1208">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8b205-1208">Az.EventGrid</span></span>
* <span data-ttu-id="8b205-1209">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8b205-1209">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8b205-1210">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-1210">New cmdlets:</span></span>
    - <span data-ttu-id="8b205-1211">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8b205-1211">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8b205-1212">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8b205-1212">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8b205-1213">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8b205-1213">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8b205-1214">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-1214">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8b205-1215">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8b205-1215">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8b205-1216">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8b205-1216">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8b205-1217">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8b205-1217">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8b205-1218">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8b205-1218">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8b205-1219">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8b205-1219">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8b205-1220">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8b205-1220">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8b205-1221">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8b205-1221">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8b205-1222">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="8b205-1222">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8b205-1223">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8b205-1223">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8b205-1224">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="8b205-1224">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="8b205-1225">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8b205-1225">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8b205-1226">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="8b205-1226">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8b205-1227">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="8b205-1227">Updated cmdlets:</span></span>
    - <span data-ttu-id="8b205-1228">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8b205-1228">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8b205-1229">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1229">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8b205-1230">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1230">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8b205-1231">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="8b205-1231">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8b205-1232">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8b205-1232">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8b205-1233">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="8b205-1233">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8b205-1234">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="8b205-1234">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8b205-1235">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="8b205-1235">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8b205-1236">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="8b205-1236">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="8b205-1237">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8b205-1237">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8b205-1238">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="8b205-1238">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8b205-1239">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8b205-1239">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8b205-1240">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1240">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8b205-1241">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1241">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-1242">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-1242">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-1243">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8b205-1243">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8b205-1244">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="8b205-1244">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8b205-1245">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8b205-1245">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8b205-1246">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="8b205-1246">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1247">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1247">Az.Network</span></span>
* <span data-ttu-id="8b205-1248">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8b205-1248">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8b205-1249">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1249">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1250">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8b205-1250">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8b205-1251">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8b205-1251">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8b205-1252">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1252">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1253">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8b205-1253">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8b205-1254">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1254">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8b205-1255">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1255">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1256">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1256">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8b205-1257">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1257">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8b205-1258">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8b205-1258">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8b205-1259">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1259">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8b205-1260">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1260">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8b205-1261">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-1261">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8b205-1262">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1262">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1263">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-1263">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8b205-1264">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-1264">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8b205-1265">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8b205-1265">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8b205-1266">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1266">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8b205-1267">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="8b205-1267">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8b205-1268">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="8b205-1268">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8b205-1269">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="8b205-1269">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8b205-1270">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8b205-1270">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8b205-1271">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8b205-1271">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8b205-1272">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="8b205-1272">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8b205-1273">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1273">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8b205-1274">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="8b205-1274">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8b205-1275">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1275">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8b205-1276">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="8b205-1276">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8b205-1277">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1277">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8b205-1278">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1278">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8b205-1279">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="8b205-1279">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8b205-1280">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8b205-1280">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8b205-1281">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-1281">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8b205-1282">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="8b205-1282">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8b205-1283">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8b205-1283">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8b205-1284">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="8b205-1284">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8b205-1285">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="8b205-1285">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="8b205-1286">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="8b205-1286">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="8b205-1287">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1287">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8b205-1288">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1288">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8b205-1289">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1289">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1290">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1290">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1291">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="8b205-1291">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1292">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1292">Az.Resources</span></span>
* <span data-ttu-id="8b205-1293">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="8b205-1293">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8b205-1294">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-1294">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8b205-1295">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-1295">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8b205-1296">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="8b205-1296">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-1297">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1297">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-1298">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="8b205-1298">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1299">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1299">Az.Sql</span></span>
* <span data-ttu-id="8b205-1300">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8b205-1300">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8b205-1301">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8b205-1301">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8b205-1302">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="8b205-1302">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8b205-1303">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8b205-1303">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8b205-1304">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8b205-1304">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8b205-1305">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8b205-1305">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8b205-1306">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8b205-1306">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8b205-1307">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8b205-1307">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1308">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1308">Az.Storage</span></span>
* <span data-ttu-id="8b205-1309">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b205-1309">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8b205-1310">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1310">New-AzStorageAccount</span></span>
* <span data-ttu-id="8b205-1311">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="8b205-1311">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8b205-1312">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1312">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1313">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1313">Az.Websites</span></span>
* <span data-ttu-id="8b205-1314">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="8b205-1314">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8b205-1315">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="8b205-1315">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8b205-1316">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1316">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8b205-1317">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-1317">Az.Cdn</span></span>
* <span data-ttu-id="8b205-1318">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="8b205-1318">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1319">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1319">Az.Compute</span></span>
* <span data-ttu-id="8b205-1320">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="8b205-1320">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8b205-1321">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8b205-1321">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-1322">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1322">Az.EventHub</span></span>
* <span data-ttu-id="8b205-1323">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="8b205-1323">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8b205-1324">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="8b205-1324">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1325">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1325">Az.Network</span></span>
* <span data-ttu-id="8b205-1326">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1326">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8b205-1327">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="8b205-1327">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-1328">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1328">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-1329">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="8b205-1329">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1330">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1330">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1331">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="8b205-1331">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-1332">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-1332">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-1333">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="8b205-1333">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-1334">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1334">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-1335">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="8b205-1335">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8b205-1336">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1336">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1337">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1337">Az.Sql</span></span>
* <span data-ttu-id="8b205-1338">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="8b205-1338">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8b205-1339">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1339">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8b205-1340">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="8b205-1340">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8b205-1341">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="8b205-1341">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1342">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1342">Az.Websites</span></span>
* <span data-ttu-id="8b205-1343">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="8b205-1343">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8b205-1344">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1344">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8b205-1345">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-1345">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-1346">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="8b205-1346">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8b205-1347">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="8b205-1347">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8b205-1348">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8b205-1348">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8b205-1349">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="8b205-1349">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8b205-1350">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1350">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8b205-1351">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="8b205-1351">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8b205-1352">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8b205-1352">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8b205-1353">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="8b205-1353">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8b205-1354">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-1354">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8b205-1355">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="8b205-1355">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8b205-1356">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="8b205-1356">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8b205-1357">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="8b205-1357">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8b205-1358">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="8b205-1358">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8b205-1359">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="8b205-1359">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8b205-1360">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="8b205-1360">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8b205-1361">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="8b205-1361">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8b205-1362">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="8b205-1362">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8b205-1363">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="8b205-1363">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8b205-1364">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="8b205-1364">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="8b205-1365">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="8b205-1365">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8b205-1366">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="8b205-1366">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8b205-1367">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="8b205-1367">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8b205-1368">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="8b205-1368">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8b205-1369">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-1369">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="8b205-1370">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="8b205-1370">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8b205-1371">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="8b205-1371">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8b205-1372">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="8b205-1372">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8b205-1373">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="8b205-1373">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8b205-1374">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="8b205-1374">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8b205-1375">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="8b205-1375">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8b205-1376">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="8b205-1376">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="8b205-1377">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8b205-1377">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8b205-1378">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="8b205-1378">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8b205-1379">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8b205-1379">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8b205-1380">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="8b205-1380">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8b205-1381">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="8b205-1381">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8b205-1382">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="8b205-1382">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8b205-1383">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="8b205-1383">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8b205-1384">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="8b205-1384">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8b205-1385">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8b205-1385">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8b205-1386">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="8b205-1386">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8b205-1387">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8b205-1387">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8b205-1388">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="8b205-1388">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8b205-1389">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="8b205-1389">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="8b205-1390">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8b205-1390">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8b205-1391">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="8b205-1391">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8b205-1392">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8b205-1392">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8b205-1393">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="8b205-1393">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="8b205-1394">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="8b205-1394">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8b205-1395">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="8b205-1395">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8b205-1396">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="8b205-1396">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8b205-1397">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="8b205-1397">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8b205-1398">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="8b205-1398">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8b205-1399">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="8b205-1399">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8b205-1400">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="8b205-1400">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8b205-1401">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="8b205-1401">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8b205-1402">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8b205-1402">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8b205-1403">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8b205-1403">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8b205-1404">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8b205-1404">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8b205-1405">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="8b205-1405">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8b205-1406">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8b205-1406">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8b205-1407">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8b205-1407">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8b205-1408">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="8b205-1408">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8b205-1409">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="8b205-1409">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8b205-1410">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="8b205-1410">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8b205-1411">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="8b205-1411">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8b205-1412">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8b205-1412">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8b205-1413">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="8b205-1413">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8b205-1414">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8b205-1414">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8b205-1415">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8b205-1415">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8b205-1416">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8b205-1416">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8b205-1417">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="8b205-1417">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8b205-1418">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="8b205-1418">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8b205-1419">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1419">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8b205-1420">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="8b205-1420">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="8b205-1421">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="8b205-1421">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8b205-1422">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="8b205-1422">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1423">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1423">Az.Automation</span></span>
* <span data-ttu-id="8b205-1424">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="8b205-1424">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8b205-1425">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8b205-1425">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8b205-1426">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8b205-1426">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8b205-1427">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="8b205-1427">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8b205-1428">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8b205-1428">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8b205-1429">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="8b205-1429">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8b205-1430">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="8b205-1430">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1431">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1431">Az.Compute</span></span>
* <span data-ttu-id="8b205-1432">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="8b205-1432">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8b205-1433">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="8b205-1433">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1434">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1434">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-1435">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1435">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-1436">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-1436">Az.Monitor</span></span>
* <span data-ttu-id="8b205-1437">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-1437">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1438">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1438">Az.Network</span></span>
* <span data-ttu-id="8b205-1439">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="8b205-1439">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8b205-1440">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="8b205-1440">Updated cmdlet:</span></span>
        - <span data-ttu-id="8b205-1441">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-1441">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8b205-1442">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8b205-1442">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1443">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1443">Az.Resources</span></span>
* <span data-ttu-id="8b205-1444">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="8b205-1444">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1445">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1445">Az.Sql</span></span>
* <span data-ttu-id="8b205-1446">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="8b205-1446">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8b205-1447">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1447">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1448">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1448">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1449">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="8b205-1449">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-1450">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1450">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-1451">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="8b205-1451">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8b205-1452">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="8b205-1452">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1453">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1453">Az.Compute</span></span>
* <span data-ttu-id="8b205-1454">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="8b205-1454">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8b205-1455">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-1455">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8b205-1456">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1456">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8b205-1457">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="8b205-1457">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8b205-1458">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="8b205-1458">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8b205-1459">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-1459">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="8b205-1460">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8b205-1460">Breaking changes</span></span>
    - <span data-ttu-id="8b205-1461">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="8b205-1461">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8b205-1462">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="8b205-1462">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8b205-1463">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8b205-1463">Az.DeploymentManager</span></span>
* <span data-ttu-id="8b205-1464">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1464">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8b205-1465">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8b205-1465">Az.Dns</span></span>
* <span data-ttu-id="8b205-1466">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="8b205-1466">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8b205-1467">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="8b205-1467">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8b205-1468">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="8b205-1468">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8b205-1469">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-1469">Az.FrontDoor</span></span>
* <span data-ttu-id="8b205-1470">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="8b205-1470">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8b205-1471">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="8b205-1471">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8b205-1472">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-1472">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-1473">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-1473">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8b205-1474">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8b205-1474">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8b205-1475">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8b205-1475">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8b205-1476">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8b205-1476">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8b205-1477">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="8b205-1477">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8b205-1478">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="8b205-1478">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8b205-1479">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="8b205-1479">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-1480">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-1480">Az.Monitor</span></span>
* <span data-ttu-id="8b205-1481">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="8b205-1481">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="8b205-1482">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8b205-1482">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8b205-1483">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-1483">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8b205-1484">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8b205-1484">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8b205-1485">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8b205-1485">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8b205-1486">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8b205-1486">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8b205-1487">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8b205-1487">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8b205-1488">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1488">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8b205-1489">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1489">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8b205-1490">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1490">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8b205-1491">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1491">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8b205-1492">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1492">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8b205-1493">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="8b205-1493">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8b205-1494">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="8b205-1494">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1495">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1495">Az.Network</span></span>
* <span data-ttu-id="8b205-1496">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="8b205-1496">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8b205-1497">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1497">New cmdlets</span></span>
        - <span data-ttu-id="8b205-1498">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1498">New-AzNatGateway</span></span>
        - <span data-ttu-id="8b205-1499">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1499">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8b205-1500">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1500">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8b205-1501">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1501">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8b205-1502">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="8b205-1502">Updated cmdlets</span></span>
        - <span data-ttu-id="8b205-1503">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8b205-1503">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8b205-1504">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8b205-1504">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8b205-1505">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1505">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8b205-1506">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1506">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8b205-1507">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="8b205-1507">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-1508">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1508">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-1509">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="8b205-1509">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8b205-1510">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="8b205-1510">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8b205-1511">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="8b205-1511">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1512">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1512">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1513">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="8b205-1513">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8b205-1514">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="8b205-1514">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8b205-1515">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="8b205-1515">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8b205-1516">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-1516">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8b205-1517">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1517">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8b205-1518">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="8b205-1518">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8b205-1519">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8b205-1519">Az.Relay</span></span>
* <span data-ttu-id="8b205-1520">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="8b205-1520">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-1521">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-1521">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-1522">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="8b205-1522">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1523">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1523">Az.Storage</span></span>
* <span data-ttu-id="8b205-1524">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="8b205-1524">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8b205-1525">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="8b205-1525">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8b205-1526">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="8b205-1526">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8b205-1527">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1527">New-AzStorageAccount</span></span>
* <span data-ttu-id="8b205-1528">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="8b205-1528">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8b205-1529">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1529">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8b205-1530">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1530">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8b205-1531">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1531">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1532">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1532">Az.Websites</span></span>
* <span data-ttu-id="8b205-1533">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1533">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8b205-1534">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="8b205-1534">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8b205-1535">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1535">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-1536">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-1536">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-1537">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8b205-1537">General availability of `Az` module</span></span>
* <span data-ttu-id="8b205-1538">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8b205-1538">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8b205-1539">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8b205-1539">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8b205-1540">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1540">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8b205-1541">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8b205-1541">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8b205-1542">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1542">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8b205-1543">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8b205-1543">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-1544">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1544">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1545">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="8b205-1545">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8b205-1546">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-1546">Az.Batch</span></span>
* <span data-ttu-id="8b205-1547">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1547">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-1548">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-1548">Az.Cdn</span></span>
* <span data-ttu-id="8b205-1549">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1549">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-1550">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1550">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-1551">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1551">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1552">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1552">Az.Compute</span></span>
* <span data-ttu-id="8b205-1553">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="8b205-1553">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8b205-1554">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1554">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1555">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8b205-1555">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1556">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1556">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1557">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="8b205-1557">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1558">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1558">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-1559">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1559">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8b205-1560">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8b205-1560">Az.EventGrid</span></span>
* <span data-ttu-id="8b205-1561">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="8b205-1561">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-1562">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1562">Az.EventHub</span></span>
* <span data-ttu-id="8b205-1563">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="8b205-1563">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="8b205-1564">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b205-1564">Az.HDInsight</span></span>
* <span data-ttu-id="8b205-1565">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1565">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-1566">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1566">Az.IotHub</span></span>
* <span data-ttu-id="8b205-1567">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1567">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-1568">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1568">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-1569">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1569">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1570">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8b205-1570">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8b205-1571">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8b205-1571">Az.MachineLearning</span></span>
* <span data-ttu-id="8b205-1572">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1572">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8b205-1573">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8b205-1573">Az.Media</span></span>
* <span data-ttu-id="8b205-1574">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1574">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-1575">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-1575">Az.Monitor</span></span>
  * <span data-ttu-id="8b205-1576">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="8b205-1576">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8b205-1577">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8b205-1577">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8b205-1578">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8b205-1578">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8b205-1579">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8b205-1579">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8b205-1580">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8b205-1580">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8b205-1581">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8b205-1581">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8b205-1582">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="8b205-1582">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1583">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1583">Az.Network</span></span>
* <span data-ttu-id="8b205-1584">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1584">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1585">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8b205-1585">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8b205-1586">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8b205-1586">Az.NotificationHubs</span></span>
* <span data-ttu-id="8b205-1587">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1587">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1588">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1588">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1589">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1589">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8b205-1590">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8b205-1590">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8b205-1591">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1591">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1592">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1592">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1593">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1593">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1594">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1594">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8b205-1595">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="8b205-1595">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8b205-1596">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="8b205-1596">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8b205-1597">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8b205-1597">Az.RedisCache</span></span>
* <span data-ttu-id="8b205-1598">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1598">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1599">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1599">Az.Resources</span></span>
* <span data-ttu-id="8b205-1600">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8b205-1600">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1601">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1601">Az.Sql</span></span>
* <span data-ttu-id="8b205-1602">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="8b205-1602">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8b205-1603">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1603">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1604">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="8b205-1604">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8b205-1605">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="8b205-1605">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8b205-1606">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="8b205-1606">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8b205-1607">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="8b205-1607">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8b205-1608">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="8b205-1608">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1609">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1609">Az.Websites</span></span>
* <span data-ttu-id="8b205-1610">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="8b205-1610">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8b205-1611">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="8b205-1611">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8b205-1612">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="8b205-1612">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8b205-1613">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="8b205-1613">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8b205-1614">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1614">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-1615">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-1615">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-1616">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8b205-1616">General availability of `Az` module</span></span>
* <span data-ttu-id="8b205-1617">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8b205-1617">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8b205-1618">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8b205-1618">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8b205-1619">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1619">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8b205-1620">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8b205-1620">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8b205-1621">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1621">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8b205-1622">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8b205-1622">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8b205-1623">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1623">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1624">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="8b205-1624">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8b205-1625">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1625">Az.AnalysisServices</span></span>
* <span data-ttu-id="8b205-1626">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="8b205-1626">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8b205-1627">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="8b205-1627">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1628">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1628">Az.Automation</span></span>
* <span data-ttu-id="8b205-1629">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="8b205-1629">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8b205-1630">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="8b205-1630">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8b205-1631">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1631">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1632">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1632">Az.Compute</span></span>
* <span data-ttu-id="8b205-1633">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1633">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8b205-1634">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="8b205-1634">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="8b205-1635">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-1635">Az.ContainerInstance</span></span>
* <span data-ttu-id="8b205-1636">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="8b205-1636">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1637">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1637">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1638">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="8b205-1638">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8b205-1639">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8b205-1639">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1640">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1640">Az.Resources</span></span>
* <span data-ttu-id="8b205-1641">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="8b205-1641">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8b205-1642">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8b205-1642">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8b205-1643">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="8b205-1643">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8b205-1644">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8b205-1644">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8b205-1645">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="8b205-1645">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8b205-1646">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8b205-1646">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1647">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1647">Az.Sql</span></span>
* <span data-ttu-id="8b205-1648">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="8b205-1648">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1649">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1649">Az.Storage</span></span>
* <span data-ttu-id="8b205-1650">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1650">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8b205-1651">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8b205-1651">New-AzStorageContext</span></span>
* <span data-ttu-id="8b205-1652">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="8b205-1652">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8b205-1653">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8b205-1653">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8b205-1654">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8b205-1654">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8b205-1655">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1655">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8b205-1656">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1656">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8b205-1657">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="8b205-1657">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8b205-1658">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8b205-1658">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8b205-1659">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8b205-1659">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8b205-1660">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8b205-1660">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8b205-1661">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8b205-1661">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8b205-1662">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1662">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8b205-1663">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="8b205-1663">Highlights since the last major release</span></span>
* <span data-ttu-id="8b205-1664">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="8b205-1664">General availability of `Az` module</span></span>
* <span data-ttu-id="8b205-1665">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8b205-1665">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8b205-1666">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8b205-1666">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8b205-1667">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1667">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8b205-1668">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8b205-1668">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8b205-1669">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1669">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8b205-1670">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="8b205-1670">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1671">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1671">Az.Automation</span></span>
* <span data-ttu-id="8b205-1672">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="8b205-1672">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8b205-1673">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="8b205-1673">Dynamic grouping</span></span>
    * <span data-ttu-id="8b205-1674">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="8b205-1674">Pre-Post script</span></span>
    * <span data-ttu-id="8b205-1675">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="8b205-1675">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1676">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1676">Az.Compute</span></span>
* <span data-ttu-id="8b205-1677">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="8b205-1677">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8b205-1678">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="8b205-1678">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-1679">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1679">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-1680">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1680">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1681">Az.Network</span></span>
* <span data-ttu-id="8b205-1682">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="8b205-1682">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8b205-1683">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8b205-1683">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1684">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1684">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1685">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="8b205-1685">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8b205-1686">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="8b205-1686">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1687">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1687">Az.Resources</span></span>
* <span data-ttu-id="8b205-1688">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-1688">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8b205-1689">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="8b205-1689">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1690">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1690">Az.Sql</span></span>
* <span data-ttu-id="8b205-1691">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="8b205-1691">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1692">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1692">Az.Storage</span></span>
* <span data-ttu-id="8b205-1693">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8b205-1693">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8b205-1694">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1694">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8b205-1695">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1695">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8b205-1696">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1696">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8b205-1697">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8b205-1697">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8b205-1698">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8b205-1698">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8b205-1699">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1699">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1700">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1700">Az.Websites</span></span>
* <span data-ttu-id="8b205-1701">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="8b205-1701">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="8b205-1702">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1702">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1703">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1703">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1704">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="8b205-1704">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8b205-1705">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1705">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1706">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1706">Az.Automation</span></span>
* <span data-ttu-id="8b205-1707">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1707">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8b205-1708">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="8b205-1708">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8b205-1709">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="8b205-1709">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-1710">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-1710">Az.Cdn</span></span>
* <span data-ttu-id="8b205-1711">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="8b205-1711">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1712">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1712">Az.Compute</span></span>
* <span data-ttu-id="8b205-1713">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="8b205-1713">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1714">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1714">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1715">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="8b205-1715">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8b205-1716">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1716">Az.LogicApp</span></span>
* <span data-ttu-id="8b205-1717">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="8b205-1717">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1718">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1718">Az.Network</span></span>
* <span data-ttu-id="8b205-1719">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1719">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1720">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1720">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1721">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-1721">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8b205-1722">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="8b205-1722">SDK Update</span></span>
* <span data-ttu-id="8b205-1723">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8b205-1723">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8b205-1724">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8b205-1724">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1725">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1725">Az.Resources</span></span>
* <span data-ttu-id="8b205-1726">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="8b205-1726">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8b205-1727">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8b205-1727">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8b205-1728">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="8b205-1728">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8b205-1729">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8b205-1729">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8b205-1730">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="8b205-1730">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8b205-1731">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8b205-1731">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1732">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1732">Az.Sql</span></span>
* <span data-ttu-id="8b205-1733">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="8b205-1733">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8b205-1734">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8b205-1734">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1735">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1735">Az.Storage</span></span>
* <span data-ttu-id="8b205-1736">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1736">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8b205-1737">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1737">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8b205-1738">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1738">Az.AnalysisServices</span></span>
* <span data-ttu-id="8b205-1739">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="8b205-1739">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1740">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1740">Az.Automation</span></span>
* <span data-ttu-id="8b205-1741">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1741">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8b205-1742">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1742">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8b205-1743">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1743">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-1744">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1744">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-1745">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="8b205-1745">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1746">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1746">Az.Compute</span></span>
* <span data-ttu-id="8b205-1747">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="8b205-1747">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8b205-1748">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="8b205-1748">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8b205-1749">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="8b205-1749">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8b205-1750">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="8b205-1750">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1751">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1751">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-1752">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="8b205-1752">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8b205-1753">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1753">Az.EventHub</span></span>
* <span data-ttu-id="8b205-1754">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="8b205-1754">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-1755">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1755">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-1756">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="8b205-1756">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8b205-1757">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1757">Az.LogicApp</span></span>
* <span data-ttu-id="8b205-1758">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8b205-1758">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8b205-1759">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="8b205-1759">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8b205-1760">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8b205-1760">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8b205-1761">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8b205-1761">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8b205-1762">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8b205-1762">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8b205-1763">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8b205-1763">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8b205-1764">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8b205-1764">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8b205-1765">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="8b205-1765">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8b205-1766">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1766">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8b205-1767">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1767">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8b205-1768">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1768">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8b205-1769">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1769">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8b205-1770">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8b205-1770">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8b205-1771">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-1771">Az.Monitor</span></span>
* <span data-ttu-id="8b205-1772">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="8b205-1772">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1773">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1773">Az.Network</span></span>
* <span data-ttu-id="8b205-1774">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="8b205-1774">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1775">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1775">Az.OperationalInsights</span></span>
* <span data-ttu-id="8b205-1776">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="8b205-1776">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8b205-1777">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8b205-1777">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="8b205-1778">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="8b205-1778">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1779">Az.Resources</span></span>
* <span data-ttu-id="8b205-1780">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8b205-1780">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8b205-1781">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8b205-1781">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8b205-1782">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8b205-1782">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8b205-1783">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="8b205-1783">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1784">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1784">Az.Sql</span></span>
* <span data-ttu-id="8b205-1785">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="8b205-1785">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8b205-1786">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="8b205-1786">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1787">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1787">Az.Websites</span></span>
* <span data-ttu-id="8b205-1788">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="8b205-1788">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8b205-1789">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1789">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1790">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1790">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1791">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8b205-1791">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8b205-1792">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1792">Az.AnalysisServices</span></span>
<span data-ttu-id="8b205-1793">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="8b205-1793">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1794">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1794">Az.Compute</span></span>
* <span data-ttu-id="8b205-1795">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="8b205-1795">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8b205-1796">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="8b205-1796">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8b205-1797">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="8b205-1797">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1798">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1798">Az.RecoveryServices</span></span>
<span data-ttu-id="8b205-1799">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="8b205-1799">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1800">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1800">Az.Resources</span></span>
* <span data-ttu-id="8b205-1801">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="8b205-1801">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="8b205-1802">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8b205-1802">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8b205-1803">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="8b205-1803">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="8b205-1804">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8b205-1804">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1805">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1805">Az.Sql</span></span>
* <span data-ttu-id="8b205-1806">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8b205-1806">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8b205-1807">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="8b205-1807">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8b205-1808">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="8b205-1808">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8b205-1809">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1809">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1810">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1810">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1811">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="8b205-1811">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8b205-1812">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1812">Az.AnalysisServices</span></span>
* <span data-ttu-id="8b205-1813">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="8b205-1813">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1814">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1814">Az.RecoveryServices</span></span>
* <span data-ttu-id="8b205-1815">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="8b205-1815">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8b205-1816">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1816">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1817">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1817">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1818">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="8b205-1818">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8b205-1819">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1819">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8b205-1820">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="8b205-1820">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8b205-1821">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8b205-1821">Az.Aks</span></span>
* <span data-ttu-id="8b205-1822">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1822">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8b205-1823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-1823">Az.Automation</span></span>
* <span data-ttu-id="8b205-1824">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="8b205-1824">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8b205-1825">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1825">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8b205-1826">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8b205-1826">Az.Cdn</span></span>
* <span data-ttu-id="8b205-1827">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1827">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1828">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1828">Az.Compute</span></span>
* <span data-ttu-id="8b205-1829">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="8b205-1829">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8b205-1830">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="8b205-1830">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8b205-1831">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="8b205-1831">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8b205-1832">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8b205-1832">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8b205-1833">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1833">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8b205-1834">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8b205-1834">Az.DataFactory</span></span>
* <span data-ttu-id="8b205-1835">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="8b205-1835">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1836">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1836">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-1837">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="8b205-1837">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8b205-1838">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8b205-1838">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8b205-1839">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1839">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-1840">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1840">Az.IotHub</span></span>
* <span data-ttu-id="8b205-1841">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="8b205-1841">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8b205-1842">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1842">Az.KeyVault</span></span>
* <span data-ttu-id="8b205-1843">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1843">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-1844">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1844">Az.Network</span></span>
* <span data-ttu-id="8b205-1845">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1845">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1846">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1846">Az.Resources</span></span>
* <span data-ttu-id="8b205-1847">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="8b205-1847">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8b205-1848">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="8b205-1848">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8b205-1849">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="8b205-1849">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8b205-1850">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8b205-1850">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8b205-1851">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8b205-1851">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8b205-1852">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="8b205-1852">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8b205-1853">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8b205-1853">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-1854">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1854">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-1855">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8b205-1855">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8b205-1856">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="8b205-1856">Fix some error messages.</span></span>
* <span data-ttu-id="8b205-1857">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="8b205-1857">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8b205-1858">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="8b205-1858">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8b205-1859">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8b205-1859">Az.SignalR</span></span>
* <span data-ttu-id="8b205-1860">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1860">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1861">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1861">Az.Sql</span></span>
* <span data-ttu-id="8b205-1862">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1862">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8b205-1863">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="8b205-1863">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8b205-1864">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="8b205-1864">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8b205-1865">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="8b205-1865">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1866">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1866">Az.Storage</span></span>
* <span data-ttu-id="8b205-1867">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1867">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8b205-1868">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="8b205-1868">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8b205-1869">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8b205-1869">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8b205-1870">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8b205-1870">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8b205-1871">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8b205-1871">Az.TrafficManager</span></span>
* <span data-ttu-id="8b205-1872">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1872">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1873">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1873">Az.Websites</span></span>
* <span data-ttu-id="8b205-1874">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="8b205-1874">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8b205-1875">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="8b205-1875">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8b205-1876">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="8b205-1876">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8b205-1877">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="8b205-1877">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8b205-1878">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1878">Az.Accounts</span></span>
* <span data-ttu-id="8b205-1879">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="8b205-1879">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-1880">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-1880">Az.Compute</span></span>
* <span data-ttu-id="8b205-1881">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="8b205-1881">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8b205-1882">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="8b205-1882">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8b205-1883">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1883">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1884">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1884">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-1885">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="8b205-1885">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8b205-1886">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="8b205-1886">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8b205-1887">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8b205-1887">Az.EventGrid</span></span>
* <span data-ttu-id="8b205-1888">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="8b205-1888">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8b205-1889">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="8b205-1889">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8b205-1890">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8b205-1890">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8b205-1891">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="8b205-1891">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8b205-1892">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="8b205-1892">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8b205-1893">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="8b205-1893">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8b205-1894">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="8b205-1894">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8b205-1895">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="8b205-1895">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8b205-1896">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="8b205-1896">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8b205-1897">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="8b205-1897">Dead letter endpoint.</span></span>
* <span data-ttu-id="8b205-1898">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="8b205-1898">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8b205-1899">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="8b205-1899">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8b205-1900">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1900">Az.IotHub</span></span>
* <span data-ttu-id="8b205-1901">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="8b205-1901">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8b205-1902">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8b205-1902">Az.LogicApp</span></span>
* <span data-ttu-id="8b205-1903">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="8b205-1903">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-1904">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1904">Az.Resources</span></span>
* <span data-ttu-id="8b205-1905">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="8b205-1905">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8b205-1906">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8b205-1906">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8b205-1907">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="8b205-1907">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8b205-1908">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="8b205-1908">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8b205-1909">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="8b205-1909">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8b205-1910">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8b205-1910">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8b205-1911">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8b205-1911">Az.SignalR</span></span>
* <span data-ttu-id="8b205-1912">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1912">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-1913">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1913">Az.Sql</span></span>
* <span data-ttu-id="8b205-1914">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="8b205-1914">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8b205-1915">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1915">Az.Storage</span></span>
* <span data-ttu-id="8b205-1916">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="8b205-1916">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8b205-1917">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8b205-1917">New-AzStorageContext</span></span>
* <span data-ttu-id="8b205-1918">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="8b205-1918">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8b205-1919">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8b205-1919">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-1920">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-1920">Az.Websites</span></span>
* <span data-ttu-id="8b205-1921">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="8b205-1921">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8b205-1922">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1922">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8b205-1923">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-1923">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8b205-1924">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-1924">General</span></span>

- <span data-ttu-id="8b205-1925">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="8b205-1925">General Availability of Az Module</span></span>
- <span data-ttu-id="8b205-1926">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="8b205-1926">Online help for each module</span></span>
- <span data-ttu-id="8b205-1927">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="8b205-1927">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8b205-1928">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="8b205-1928">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8b205-1929">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1929">Az.Accounts</span></span>
- <span data-ttu-id="8b205-1930">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8b205-1930">Changed from Az.Profile</span></span>
- <span data-ttu-id="8b205-1931">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="8b205-1931">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8b205-1932">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-1932">Az.ApiManagement</span></span>
- <span data-ttu-id="8b205-1933">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="8b205-1933">Fixes for #7002</span></span>
- <span data-ttu-id="8b205-1934">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1934">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8b205-1935">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8b205-1935">Az.Batch</span></span>
- <span data-ttu-id="8b205-1936">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="8b205-1936">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8b205-1937">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="8b205-1937">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8b205-1938">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1938">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8b205-1939">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8b205-1939">Az.Billing</span></span>
- <span data-ttu-id="8b205-1940">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1940">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8b205-1941">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1941">Az.CognitivServices</span></span>
- <span data-ttu-id="8b205-1942">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-1942">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8b205-1943">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="8b205-1943">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8b205-1944">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-1944">Az.ContainerInstance</span></span>
- <span data-ttu-id="8b205-1945">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="8b205-1945">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8b205-1946">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8b205-1946">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8b205-1947">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1947">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8b205-1948">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-1948">Az.DataLakeStore</span></span>
- <span data-ttu-id="8b205-1949">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1949">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8b205-1950">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8b205-1950">Az.Monitor</span></span>
- <span data-ttu-id="8b205-1951">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1951">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8b205-1952">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8b205-1952">Az.KeyVault</span></span>
- <span data-ttu-id="8b205-1953">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="8b205-1953">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8b205-1954">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8b205-1954">Az.MachineLearning</span></span>
- <span data-ttu-id="8b205-1955">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="8b205-1955">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8b205-1956">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8b205-1956">Az.Media</span></span>
- <span data-ttu-id="8b205-1957">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="8b205-1957">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8b205-1958">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-1958">Az.Network</span></span>
<span data-ttu-id="8b205-1959">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="8b205-1959">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8b205-1960">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="8b205-1960">New cmdlets added:</span></span>
        - <span data-ttu-id="8b205-1961">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1961">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1962">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1962">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1963">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1963">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1964">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1964">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1965">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1965">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1966">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1966">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8b205-1967">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1967">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8b205-1968">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b205-1968">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8b205-1969">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8b205-1969">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8b205-1970">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8b205-1970">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8b205-1971">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1971">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8b205-1972">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8b205-1972">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8b205-1973">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1973">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8b205-1974">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-1974">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8b205-1975">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="8b205-1975">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8b205-1976">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="8b205-1976">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8b205-1977">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8b205-1977">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8b205-1978">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8b205-1978">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8b205-1979">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8b205-1979">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8b205-1980">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="8b205-1980">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8b205-1981">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1981">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8b205-1982">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-1982">Az.OperationalInsights</span></span>
- <span data-ttu-id="8b205-1983">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1983">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8b205-1984">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8b205-1984">Az.Profile</span></span>
- <span data-ttu-id="8b205-1985">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8b205-1985">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-1986">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-1986">Az.RecoveryServices</span></span>
- <span data-ttu-id="8b205-1987">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1987">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8b205-1988">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-1988">Az.Resources</span></span>
- <span data-ttu-id="8b205-1989">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1989">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8b205-1990">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-1990">Az.ServiceFabric</span></span>
- <span data-ttu-id="8b205-1991">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="8b205-1991">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8b205-1992">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1992">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8b205-1993">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8b205-1993">Az.SIgnalR</span></span>
- <span data-ttu-id="8b205-1994">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="8b205-1994">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8b205-1995">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-1995">Az.Sql</span></span>
- <span data-ttu-id="8b205-1996">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="8b205-1996">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8b205-1997">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="8b205-1997">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8b205-1998">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-1998">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8b205-1999">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-1999">Az.Storage</span></span>
- <span data-ttu-id="8b205-2000">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-2000">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8b205-2001">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-2001">Az.Websites</span></span>
- <span data-ttu-id="8b205-2002">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="8b205-2002">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8b205-2003">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2003">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8b205-2004">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-2004">General</span></span>

* <span data-ttu-id="8b205-2005">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8b205-2005">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8b205-2006">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-2006">Az.Compute</span></span>

* <span data-ttu-id="8b205-2007">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="8b205-2007">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8b205-2008">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-2008">Az.DataLakeStore</span></span>

* <span data-ttu-id="8b205-2009">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="8b205-2009">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8b205-2010">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8b205-2010">Az.FrontDoor</span></span>

* <span data-ttu-id="8b205-2011">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="8b205-2011">Fixed some broken links</span></span>
    - <span data-ttu-id="8b205-2012">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="8b205-2012">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8b205-2013">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="8b205-2013">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8b205-2014">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8b205-2014">Az.RecoveryServices</span></span>

* <span data-ttu-id="8b205-2015">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-2015">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8b205-2016">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="8b205-2016">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8b205-2017">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-2017">Az.Resources</span></span>

* <span data-ttu-id="8b205-2018">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="8b205-2018">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8b205-2019">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="8b205-2019">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8b205-2020">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-2020">Az.Sql</span></span>

* <span data-ttu-id="8b205-2021">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="8b205-2021">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8b205-2022">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="8b205-2022">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8b205-2023">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="8b205-2023">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8b205-2024">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-2024">Az.Storage</span></span>

* <span data-ttu-id="8b205-2025">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8b205-2025">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8b205-2026">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="8b205-2026">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8b205-2027">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-2027">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8b205-2028">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="8b205-2028">Support Static Website configuration</span></span>
    - <span data-ttu-id="8b205-2029">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8b205-2029">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8b205-2030">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8b205-2030">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8b205-2031">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-2031">Az.Websites</span></span>

* <span data-ttu-id="8b205-2032">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8b205-2032">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="8b205-2033">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="8b205-2033">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8b205-2034">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-2034">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8b205-2035">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2035">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8b205-2036">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8b205-2036">Az.ApiManagement</span></span>
* <span data-ttu-id="8b205-2037">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8b205-2037">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8b205-2038">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8b205-2038">Az.Automation</span></span>
* <span data-ttu-id="8b205-2039">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="8b205-2039">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8b205-2040">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="8b205-2040">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8b205-2041">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="8b205-2041">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8b205-2042">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="8b205-2042">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8b205-2043">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="8b205-2043">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8b205-2044">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-2044">Az.Compute</span></span>
* <span data-ttu-id="8b205-2045">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="8b205-2045">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8b205-2046">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8b205-2046">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8b205-2047">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-2047">Az.ContainerInstance</span></span>
* <span data-ttu-id="8b205-2048">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8b205-2048">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8b205-2049">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8b205-2049">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8b205-2050">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="8b205-2050">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8b205-2051">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-2051">Az.Network</span></span>
* <span data-ttu-id="8b205-2052">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="8b205-2052">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8b205-2053">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="8b205-2053">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8b205-2054">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="8b205-2054">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="8b205-2055">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="8b205-2055">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8b205-2056">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8b205-2056">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8b205-2057">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="8b205-2057">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8b205-2058">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="8b205-2058">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8b205-2059">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8b205-2059">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8b205-2060">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8b205-2060">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8b205-2061">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="8b205-2061">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8b205-2062">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8b205-2062">Az.Relay</span></span>
* <span data-ttu-id="8b205-2063">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="8b205-2063">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8b205-2064">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-2064">Az.Resources</span></span>
* <span data-ttu-id="8b205-2065">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="8b205-2065">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8b205-2066">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="8b205-2066">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8b205-2067">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8b205-2067">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8b205-2068">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-2068">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-2069">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="8b205-2069">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8b205-2070">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-2070">Az.Sql</span></span>
* <span data-ttu-id="8b205-2071">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-2071">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8b205-2072">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-2072">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8b205-2073">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-2073">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8b205-2074">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-2074">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8b205-2075">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8b205-2075">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8b205-2076">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8b205-2076">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8b205-2077">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8b205-2077">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8b205-2078">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8b205-2078">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8b205-2079">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8b205-2079">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8b205-2080">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="8b205-2080">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8b205-2081">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="8b205-2081">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8b205-2082">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="8b205-2082">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8b205-2083">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="8b205-2083">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8b205-2084">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="8b205-2084">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8b205-2085">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="8b205-2085">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8b205-2086">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="8b205-2086">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8b205-2087">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="8b205-2087">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8b205-2088">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2088">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8b205-2089">Geral</span><span class="sxs-lookup"><span data-stu-id="8b205-2089">General</span></span>
* <span data-ttu-id="8b205-2090">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="8b205-2090">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8b205-2091">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8b205-2091">Az.Profile</span></span>
* <span data-ttu-id="8b205-2092">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8b205-2092">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8b205-2093">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="8b205-2093">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8b205-2094">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="8b205-2094">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8b205-2095">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="8b205-2095">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8b205-2096">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="8b205-2096">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8b205-2097">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="8b205-2097">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8b205-2098">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="8b205-2098">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-2099">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-2099">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-2100">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="8b205-2100">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-2101">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-2101">Az.Compute</span></span>
* <span data-ttu-id="8b205-2102">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="8b205-2102">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8b205-2103">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="8b205-2103">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8b205-2104">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="8b205-2104">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-2105">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-2105">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-2106">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="8b205-2106">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8b205-2107">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="8b205-2107">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8b205-2108">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8b205-2108">Az.Insights</span></span>
* <span data-ttu-id="8b205-2109">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="8b205-2109">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8b205-2110">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="8b205-2110">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8b205-2111">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="8b205-2111">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8b205-2112">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="8b205-2112">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-2113">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-2113">Az.Network</span></span>
* <span data-ttu-id="8b205-2114">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="8b205-2114">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8b205-2115">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-2115">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8b205-2116">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8b205-2116">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8b205-2117">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8b205-2117">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8b205-2118">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8b205-2118">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8b205-2119">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8b205-2119">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8b205-2120">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8b205-2120">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8b205-2121">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8b205-2121">Az.PolicyInsights</span></span>
* <span data-ttu-id="8b205-2122">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="8b205-2122">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-2123">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-2123">Az.Resources</span></span>
* <span data-ttu-id="8b205-2124">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="8b205-2124">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8b205-2125">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="8b205-2125">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8b205-2126">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8b205-2126">Az.ServiceBus</span></span>
* <span data-ttu-id="8b205-2127">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="8b205-2127">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8b205-2128">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8b205-2128">Az.ServiceFabric</span></span>
* <span data-ttu-id="8b205-2129">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b205-2129">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8b205-2130">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="8b205-2130">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8b205-2131">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="8b205-2131">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8b205-2132">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="8b205-2132">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8b205-2133">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="8b205-2133">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8b205-2134">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2134">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8b205-2135">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8b205-2135">Az.Profile</span></span>
* <span data-ttu-id="8b205-2136">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="8b205-2136">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8b205-2137">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="8b205-2137">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-2138">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-2138">Az.Compute</span></span>
* <span data-ttu-id="8b205-2139">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="8b205-2139">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8b205-2140">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8b205-2140">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8b205-2141">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8b205-2141">Az.DataLakeStore</span></span>
* <span data-ttu-id="8b205-2142">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="8b205-2142">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8b205-2143">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-2143">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8b205-2144">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8b205-2144">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8b205-2145">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="8b205-2145">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8b205-2146">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="8b205-2146">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-2147">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-2147">Az.Network</span></span>
* <span data-ttu-id="8b205-2148">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="8b205-2148">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8b205-2149">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="8b205-2149">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-2150">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-2150">Az.Resources</span></span>
* <span data-ttu-id="8b205-2151">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="8b205-2151">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8b205-2152">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="8b205-2152">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8b205-2153">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2153">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8b205-2154">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8b205-2154">Azure.Storage</span></span>
* <span data-ttu-id="8b205-2155">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="8b205-2155">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8b205-2156">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-2156">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8b205-2157">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8b205-2157">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8b205-2158">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="8b205-2158">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8b205-2159">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8b205-2159">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8b205-2160">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8b205-2160">Az.CognitiveServices</span></span>
* <span data-ttu-id="8b205-2161">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="8b205-2161">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8b205-2162">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8b205-2162">Az.Compute</span></span>
* <span data-ttu-id="8b205-2163">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="8b205-2163">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8b205-2164">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="8b205-2164">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8b205-2165">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="8b205-2165">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8b205-2166">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8b205-2166">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8b205-2167">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="8b205-2167">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8b205-2168">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8b205-2168">Az.Network</span></span>
* <span data-ttu-id="8b205-2169">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="8b205-2169">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8b205-2170">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="8b205-2170">new cmdlets added</span></span>
    - <span data-ttu-id="8b205-2171">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8b205-2171">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8b205-2172">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8b205-2172">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8b205-2173">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8b205-2173">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8b205-2174">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8b205-2174">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8b205-2175">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-2175">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8b205-2176">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-2176">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8b205-2177">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="8b205-2177">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8b205-2178">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="8b205-2178">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8b205-2179">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="8b205-2179">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8b205-2180">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8b205-2180">Az.RedisCache</span></span>
* <span data-ttu-id="8b205-2181">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="8b205-2181">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8b205-2182">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="8b205-2182">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8b205-2183">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8b205-2183">Az.Resources</span></span>
* <span data-ttu-id="8b205-2184">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="8b205-2184">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8b205-2185">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="8b205-2185">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8b205-2186">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8b205-2186">Az.Sql</span></span>
* <span data-ttu-id="8b205-2187">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="8b205-2187">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8b205-2188">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8b205-2188">Az.Websites</span></span>
* <span data-ttu-id="8b205-2189">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="8b205-2189">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8b205-2190">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="8b205-2190">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8b205-2191">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8b205-2191">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8b205-2192">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="8b205-2192">Initial Release</span></span>
