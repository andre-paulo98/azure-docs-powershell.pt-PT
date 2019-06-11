---
ms.openlocfilehash: 911e1f7ff56feab2735f397a0128aab4aa7757c7
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498680"
---
## <a name="220---june-2019"></a><span data-ttu-id="955ed-101">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-101">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="955ed-102">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="955ed-102">Az.Cdn</span></span>
* <span data-ttu-id="955ed-103">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="955ed-103">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-104">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-104">Az.Compute</span></span>
* <span data-ttu-id="955ed-105">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="955ed-105">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="955ed-106">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="955ed-106">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="955ed-107">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="955ed-107">Az.EventHub</span></span>
* <span data-ttu-id="955ed-108">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="955ed-108">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="955ed-109">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="955ed-109">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-110">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-110">Az.Network</span></span>
* <span data-ttu-id="955ed-111">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="955ed-111">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="955ed-112">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="955ed-112">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="955ed-113">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-113">Az.PolicyInsights</span></span>
* <span data-ttu-id="955ed-114">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="955ed-114">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-115">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-115">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-116">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="955ed-116">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="955ed-117">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="955ed-117">Az.ServiceBus</span></span>
* <span data-ttu-id="955ed-118">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="955ed-118">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="955ed-119">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="955ed-119">Az.ServiceFabric</span></span>
* <span data-ttu-id="955ed-120">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="955ed-120">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="955ed-121">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="955ed-121">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-122">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-122">Az.Sql</span></span>
* <span data-ttu-id="955ed-123">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="955ed-123">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="955ed-124">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-124">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="955ed-125">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="955ed-125">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="955ed-126">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="955ed-126">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-127">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-127">Az.Websites</span></span>
* <span data-ttu-id="955ed-128">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="955ed-128">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="955ed-129">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-129">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="955ed-130">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="955ed-130">Az.ApiManagement</span></span>
* <span data-ttu-id="955ed-131">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="955ed-131">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="955ed-132">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="955ed-132">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="955ed-133">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="955ed-133">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="955ed-134">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="955ed-134">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="955ed-135">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="955ed-135">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="955ed-136">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="955ed-136">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="955ed-137">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="955ed-137">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="955ed-138">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="955ed-138">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="955ed-139">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="955ed-139">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="955ed-140">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="955ed-140">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="955ed-141">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="955ed-141">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="955ed-142">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="955ed-142">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="955ed-143">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="955ed-143">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="955ed-144">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="955ed-144">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="955ed-145">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="955ed-145">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="955ed-146">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="955ed-146">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="955ed-147">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="955ed-147">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="955ed-148">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="955ed-148">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="955ed-149">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="955ed-149">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="955ed-150">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="955ed-150">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="955ed-151">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="955ed-151">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="955ed-152">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="955ed-152">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="955ed-153">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="955ed-153">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="955ed-154">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="955ed-154">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="955ed-155">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="955ed-155">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="955ed-156">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="955ed-156">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="955ed-157">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="955ed-157">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="955ed-158">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="955ed-158">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="955ed-159">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="955ed-159">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="955ed-160">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="955ed-160">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="955ed-161">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="955ed-161">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="955ed-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="955ed-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="955ed-163">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="955ed-163">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="955ed-164">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="955ed-164">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="955ed-165">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="955ed-165">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="955ed-166">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="955ed-166">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="955ed-167">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="955ed-167">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="955ed-168">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="955ed-168">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="955ed-169">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="955ed-169">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="955ed-170">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="955ed-170">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="955ed-171">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="955ed-171">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="955ed-172">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="955ed-172">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="955ed-173">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="955ed-173">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="955ed-174">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="955ed-174">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="955ed-175">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="955ed-175">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="955ed-176">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="955ed-176">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="955ed-177">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="955ed-177">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="955ed-178">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="955ed-178">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="955ed-179">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="955ed-179">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="955ed-180">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="955ed-180">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="955ed-181">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="955ed-181">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="955ed-182">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="955ed-182">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="955ed-183">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="955ed-183">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="955ed-184">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="955ed-184">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="955ed-185">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="955ed-185">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="955ed-186">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="955ed-186">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="955ed-187">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="955ed-187">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="955ed-188">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="955ed-188">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="955ed-189">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="955ed-189">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="955ed-190">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="955ed-190">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="955ed-191">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="955ed-191">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="955ed-192">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="955ed-192">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="955ed-193">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="955ed-193">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="955ed-194">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="955ed-194">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="955ed-195">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="955ed-195">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="955ed-196">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="955ed-196">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="955ed-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="955ed-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="955ed-198">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="955ed-198">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="955ed-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="955ed-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="955ed-200">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="955ed-200">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="955ed-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="955ed-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="955ed-202">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="955ed-202">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="955ed-203">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="955ed-203">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="955ed-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="955ed-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="955ed-205">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="955ed-205">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="955ed-206">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="955ed-206">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="955ed-207">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="955ed-207">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-208">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-208">Az.Automation</span></span>
* <span data-ttu-id="955ed-209">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="955ed-209">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="955ed-210">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="955ed-210">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="955ed-211">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="955ed-211">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="955ed-212">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="955ed-212">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="955ed-213">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="955ed-213">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="955ed-214">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="955ed-214">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="955ed-215">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="955ed-215">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-216">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-216">Az.Compute</span></span>
* <span data-ttu-id="955ed-217">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="955ed-217">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="955ed-218">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="955ed-218">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-219">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-219">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-220">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-220">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="955ed-221">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="955ed-221">Az.Monitor</span></span>
* <span data-ttu-id="955ed-222">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="955ed-222">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-223">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-223">Az.Network</span></span>
* <span data-ttu-id="955ed-224">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="955ed-224">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="955ed-225">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="955ed-225">Updated cmdlet:</span></span>
        - <span data-ttu-id="955ed-226">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="955ed-226">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="955ed-227">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="955ed-227">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-228">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-228">Az.Resources</span></span>
* <span data-ttu-id="955ed-229">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="955ed-229">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-230">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-230">Az.Sql</span></span>
* <span data-ttu-id="955ed-231">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="955ed-231">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="955ed-232">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-232">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-233">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-233">Az.Accounts</span></span>
* <span data-ttu-id="955ed-234">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="955ed-234">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="955ed-235">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="955ed-235">Az.CognitiveServices</span></span>
* <span data-ttu-id="955ed-236">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="955ed-236">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="955ed-237">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="955ed-237">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-238">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-238">Az.Compute</span></span>
* <span data-ttu-id="955ed-239">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="955ed-239">Proximity placement group feature.</span></span>
    - <span data-ttu-id="955ed-240">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="955ed-240">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="955ed-241">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-241">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="955ed-242">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="955ed-242">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="955ed-243">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="955ed-243">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="955ed-244">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="955ed-244">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="955ed-245">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="955ed-245">Breaking changes</span></span>
    - <span data-ttu-id="955ed-246">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="955ed-246">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="955ed-247">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="955ed-247">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="955ed-248">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="955ed-248">Az.DeploymentManager</span></span>
* <span data-ttu-id="955ed-249">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-249">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="955ed-250">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="955ed-250">Az.Dns</span></span>
* <span data-ttu-id="955ed-251">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="955ed-251">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="955ed-252">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="955ed-252">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="955ed-253">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="955ed-253">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="955ed-254">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="955ed-254">Az.FrontDoor</span></span>
* <span data-ttu-id="955ed-255">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="955ed-255">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="955ed-256">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="955ed-256">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="955ed-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="955ed-257">Az.HDInsight</span></span>
* <span data-ttu-id="955ed-258">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="955ed-258">Removed two cmdlets:</span></span>
    - <span data-ttu-id="955ed-259">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="955ed-259">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="955ed-260">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="955ed-260">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="955ed-261">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="955ed-261">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="955ed-262">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="955ed-262">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="955ed-263">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="955ed-263">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="955ed-264">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="955ed-264">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="955ed-265">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="955ed-265">Az.Monitor</span></span>
* <span data-ttu-id="955ed-266">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="955ed-266">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="955ed-267">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="955ed-267">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="955ed-268">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="955ed-268">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="955ed-269">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="955ed-269">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="955ed-270">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="955ed-270">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="955ed-271">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="955ed-271">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="955ed-272">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="955ed-272">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="955ed-273">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="955ed-273">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="955ed-274">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="955ed-274">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="955ed-275">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="955ed-275">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="955ed-276">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="955ed-276">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="955ed-277">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="955ed-277">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="955ed-278">[Mais](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="955ed-278">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="955ed-279">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="955ed-279">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-280">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-280">Az.Network</span></span>
* <span data-ttu-id="955ed-281">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="955ed-281">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="955ed-282">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="955ed-282">New cmdlets</span></span>
        - <span data-ttu-id="955ed-283">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="955ed-283">New-AzNatGateway</span></span>
        - <span data-ttu-id="955ed-284">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="955ed-284">Get-AzNatGateway</span></span>
        - <span data-ttu-id="955ed-285">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="955ed-285">Set-AzNatGateway</span></span>
        - <span data-ttu-id="955ed-286">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="955ed-286">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="955ed-287">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="955ed-287">Updated cmdlets</span></span>
        - <span data-ttu-id="955ed-288">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="955ed-288">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="955ed-289">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="955ed-289">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="955ed-290">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="955ed-290">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="955ed-291">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="955ed-291">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="955ed-292">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="955ed-292">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="955ed-293">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-293">Az.PolicyInsights</span></span>
* <span data-ttu-id="955ed-294">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="955ed-294">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="955ed-295">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="955ed-295">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="955ed-296">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="955ed-296">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-297">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-297">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-298">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="955ed-298">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="955ed-299">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="955ed-299">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="955ed-300">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="955ed-300">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="955ed-301">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="955ed-301">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="955ed-302">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="955ed-302">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="955ed-303">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="955ed-303">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="955ed-304">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="955ed-304">Az.Relay</span></span>
* <span data-ttu-id="955ed-305">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="955ed-305">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="955ed-306">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="955ed-306">Az.ServiceBus</span></span>
* <span data-ttu-id="955ed-307">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="955ed-307">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-308">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-308">Az.Storage</span></span>
* <span data-ttu-id="955ed-309">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="955ed-309">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="955ed-310">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="955ed-310">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="955ed-311">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="955ed-311">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="955ed-312">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-312">New-AzStorageAccount</span></span>
* <span data-ttu-id="955ed-313">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="955ed-313">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="955ed-314">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-314">New-AzStorageAccount</span></span>
    - <span data-ttu-id="955ed-315">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-315">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="955ed-316">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-316">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-317">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-317">Az.Websites</span></span>
* <span data-ttu-id="955ed-318">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="955ed-318">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="955ed-319">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="955ed-319">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="955ed-320">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-320">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="955ed-321">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="955ed-321">Highlights since the last major release</span></span>
* <span data-ttu-id="955ed-322">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="955ed-322">General availability of `Az` module</span></span>
* <span data-ttu-id="955ed-323">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="955ed-323">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="955ed-324">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="955ed-324">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="955ed-325">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-325">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="955ed-326">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="955ed-326">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="955ed-327">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-327">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="955ed-328">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="955ed-328">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="955ed-329">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-329">Az.Accounts</span></span>
* <span data-ttu-id="955ed-330">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="955ed-330">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="955ed-331">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="955ed-331">Az.Batch</span></span>
* <span data-ttu-id="955ed-332">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-332">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="955ed-333">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="955ed-333">Az.Cdn</span></span>
* <span data-ttu-id="955ed-334">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-334">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="955ed-335">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="955ed-335">Az.CognitiveServices</span></span>
* <span data-ttu-id="955ed-336">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-336">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-337">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-337">Az.Compute</span></span>
* <span data-ttu-id="955ed-338">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="955ed-338">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="955ed-339">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-339">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-340">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="955ed-340">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="955ed-341">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="955ed-341">Az.DataFactory</span></span>
* <span data-ttu-id="955ed-342">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="955ed-342">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-343">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-344">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-344">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="955ed-345">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="955ed-345">Az.EventGrid</span></span>
* <span data-ttu-id="955ed-346">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="955ed-346">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="955ed-347">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="955ed-347">Az.EventHub</span></span>
* <span data-ttu-id="955ed-348">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="955ed-348">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="955ed-349">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="955ed-349">Az.HDInsight</span></span>
* <span data-ttu-id="955ed-350">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-350">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="955ed-351">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="955ed-351">Az.IotHub</span></span>
* <span data-ttu-id="955ed-352">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-352">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="955ed-353">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-353">Az.KeyVault</span></span>
* <span data-ttu-id="955ed-354">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-354">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-355">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="955ed-355">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="955ed-356">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="955ed-356">Az.MachineLearning</span></span>
* <span data-ttu-id="955ed-357">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-357">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="955ed-358">Az.Media</span><span class="sxs-lookup"><span data-stu-id="955ed-358">Az.Media</span></span>
* <span data-ttu-id="955ed-359">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-359">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="955ed-360">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="955ed-360">Az.Monitor</span></span>
  * <span data-ttu-id="955ed-361">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="955ed-361">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="955ed-362">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="955ed-362">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="955ed-363">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="955ed-363">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="955ed-364">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="955ed-364">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="955ed-365">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="955ed-365">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="955ed-366">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="955ed-366">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="955ed-367">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="955ed-367">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-368">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-368">Az.Network</span></span>
* <span data-ttu-id="955ed-369">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-370">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="955ed-370">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="955ed-371">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="955ed-371">Az.NotificationHubs</span></span>
* <span data-ttu-id="955ed-372">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-372">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="955ed-373">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-373">Az.OperationalInsights</span></span>
* <span data-ttu-id="955ed-374">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-374">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="955ed-375">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="955ed-375">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="955ed-376">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-376">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-377">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-377">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-378">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-378">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-379">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-379">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="955ed-380">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="955ed-380">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="955ed-381">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="955ed-381">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="955ed-382">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="955ed-382">Az.RedisCache</span></span>
* <span data-ttu-id="955ed-383">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-383">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-384">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-384">Az.Resources</span></span>
* <span data-ttu-id="955ed-385">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="955ed-385">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-386">Az.Sql</span></span>
* <span data-ttu-id="955ed-387">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="955ed-387">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="955ed-388">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-388">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-389">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="955ed-389">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="955ed-390">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="955ed-390">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="955ed-391">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="955ed-391">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="955ed-392">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="955ed-392">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="955ed-393">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="955ed-393">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-394">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-394">Az.Websites</span></span>
* <span data-ttu-id="955ed-395">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="955ed-395">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="955ed-396">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="955ed-396">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="955ed-397">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="955ed-397">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="955ed-398">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="955ed-398">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="955ed-399">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-399">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="955ed-400">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="955ed-400">Highlights since the last major release</span></span>
* <span data-ttu-id="955ed-401">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="955ed-401">General availability of `Az` module</span></span>
* <span data-ttu-id="955ed-402">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="955ed-402">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="955ed-403">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="955ed-403">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="955ed-404">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-404">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="955ed-405">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="955ed-405">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="955ed-406">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-406">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="955ed-407">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="955ed-407">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="955ed-408">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-408">Az.Accounts</span></span>
* <span data-ttu-id="955ed-409">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="955ed-409">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="955ed-410">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="955ed-410">Az.AnalysisServices</span></span>
* <span data-ttu-id="955ed-411">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="955ed-411">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="955ed-412">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="955ed-412">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-413">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-413">Az.Automation</span></span>
* <span data-ttu-id="955ed-414">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="955ed-414">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="955ed-415">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="955ed-415">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="955ed-416">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="955ed-416">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-417">Az.Compute</span></span>
* <span data-ttu-id="955ed-418">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-418">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="955ed-419">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="955ed-419">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="955ed-420">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-420">Az.ContainerInstance</span></span>
* <span data-ttu-id="955ed-421">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="955ed-421">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="955ed-422">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="955ed-422">Az.DataFactory</span></span>
* <span data-ttu-id="955ed-423">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="955ed-423">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="955ed-424">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="955ed-424">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-425">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-425">Az.Resources</span></span>
* <span data-ttu-id="955ed-426">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="955ed-426">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="955ed-427">Melhor processamento de erros de "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="955ed-427">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="955ed-428">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="955ed-428">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="955ed-429">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="955ed-429">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="955ed-430">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="955ed-430">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="955ed-431">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="955ed-431">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-432">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-432">Az.Sql</span></span>
* <span data-ttu-id="955ed-433">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="955ed-433">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-434">Az.Storage</span></span>
* <span data-ttu-id="955ed-435">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-435">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="955ed-436">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="955ed-436">New-AzStorageContext</span></span>
* <span data-ttu-id="955ed-437">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="955ed-437">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="955ed-438">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="955ed-438">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="955ed-439">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="955ed-439">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="955ed-440">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-440">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="955ed-441">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-441">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="955ed-442">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="955ed-442">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="955ed-443">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="955ed-443">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="955ed-444">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="955ed-444">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="955ed-445">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="955ed-445">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="955ed-446">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="955ed-446">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="955ed-447">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-447">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="955ed-448">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="955ed-448">Highlights since the last major release</span></span>
* <span data-ttu-id="955ed-449">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="955ed-449">General availability of `Az` module</span></span>
* <span data-ttu-id="955ed-450">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="955ed-450">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="955ed-451">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="955ed-451">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="955ed-452">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-452">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="955ed-453">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="955ed-453">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="955ed-454">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-454">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="955ed-455">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="955ed-455">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-456">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-456">Az.Automation</span></span>
* <span data-ttu-id="955ed-457">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="955ed-457">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="955ed-458">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="955ed-458">Dynamic grouping</span></span>
    * <span data-ttu-id="955ed-459">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="955ed-459">Pre-Post script</span></span>
    * <span data-ttu-id="955ed-460">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="955ed-460">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-461">Az.Compute</span></span>
* <span data-ttu-id="955ed-462">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="955ed-462">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="955ed-463">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="955ed-463">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="955ed-464">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-464">Az.KeyVault</span></span>
* <span data-ttu-id="955ed-465">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-465">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-466">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-466">Az.Network</span></span>
* <span data-ttu-id="955ed-467">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="955ed-467">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="955ed-468">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="955ed-468">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-469">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-470">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="955ed-470">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="955ed-471">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="955ed-471">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-472">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-472">Az.Resources</span></span>
* <span data-ttu-id="955ed-473">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="955ed-473">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="955ed-474">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="955ed-474">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-475">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-475">Az.Sql</span></span>
* <span data-ttu-id="955ed-476">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="955ed-476">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-477">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-477">Az.Storage</span></span>
* <span data-ttu-id="955ed-478">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="955ed-478">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="955ed-479">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-479">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="955ed-480">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-480">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="955ed-481">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-481">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="955ed-482">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="955ed-482">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="955ed-483">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="955ed-483">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="955ed-484">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="955ed-484">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-485">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-485">Az.Websites</span></span>
* <span data-ttu-id="955ed-486">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="955ed-486">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="955ed-487">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-487">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-488">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-488">Az.Accounts</span></span>
* <span data-ttu-id="955ed-489">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="955ed-489">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="955ed-490">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-490">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-491">Az.Automation</span></span>
* <span data-ttu-id="955ed-492">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-492">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="955ed-493">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="955ed-493">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="955ed-494">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="955ed-494">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="955ed-495">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="955ed-495">Az.Cdn</span></span>
* <span data-ttu-id="955ed-496">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="955ed-496">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-497">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-497">Az.Compute</span></span>
* <span data-ttu-id="955ed-498">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="955ed-498">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="955ed-499">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="955ed-499">Az.DataFactory</span></span>
* <span data-ttu-id="955ed-500">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="955ed-500">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="955ed-501">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="955ed-501">Az.LogicApp</span></span>
* <span data-ttu-id="955ed-502">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="955ed-502">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-503">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-503">Az.Network</span></span>
* <span data-ttu-id="955ed-504">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="955ed-504">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-505">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-505">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-506">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-506">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="955ed-507">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="955ed-507">SDK Update</span></span>
* <span data-ttu-id="955ed-508">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="955ed-508">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="955ed-509">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="955ed-509">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-510">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-510">Az.Resources</span></span>
* <span data-ttu-id="955ed-511">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="955ed-511">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="955ed-512">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="955ed-512">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="955ed-513">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="955ed-513">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="955ed-514">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="955ed-514">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="955ed-515">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="955ed-515">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="955ed-516">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="955ed-516">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-517">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-517">Az.Sql</span></span>
* <span data-ttu-id="955ed-518">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="955ed-518">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="955ed-519">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="955ed-519">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-520">Az.Storage</span></span>
* <span data-ttu-id="955ed-521">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-521">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="955ed-522">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-522">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="955ed-523">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="955ed-523">Az.AnalysisServices</span></span>
* <span data-ttu-id="955ed-524">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="955ed-524">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-525">Az.Automation</span></span>
* <span data-ttu-id="955ed-526">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-526">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="955ed-527">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-527">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="955ed-528">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-528">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="955ed-529">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="955ed-529">Az.CognitiveServices</span></span>
* <span data-ttu-id="955ed-530">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="955ed-530">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-531">Az.Compute</span></span>
* <span data-ttu-id="955ed-532">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="955ed-532">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="955ed-533">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="955ed-533">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="955ed-534">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="955ed-534">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="955ed-535">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="955ed-535">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-536">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-537">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="955ed-537">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="955ed-538">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="955ed-538">Az.EventHub</span></span>
* <span data-ttu-id="955ed-539">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="955ed-539">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="955ed-540">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-540">Az.KeyVault</span></span>
* <span data-ttu-id="955ed-541">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="955ed-541">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="955ed-542">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="955ed-542">Az.LogicApp</span></span>
* <span data-ttu-id="955ed-543">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="955ed-543">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="955ed-544">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="955ed-544">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="955ed-545">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="955ed-545">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="955ed-546">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="955ed-546">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="955ed-547">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="955ed-547">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="955ed-548">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="955ed-548">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="955ed-549">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="955ed-549">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="955ed-550">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="955ed-550">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="955ed-551">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-551">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="955ed-552">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-552">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="955ed-553">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-553">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="955ed-554">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-554">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="955ed-555">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="955ed-555">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="955ed-556">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="955ed-556">Az.Monitor</span></span>
* <span data-ttu-id="955ed-557">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="955ed-557">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-558">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-558">Az.Network</span></span>
* <span data-ttu-id="955ed-559">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="955ed-559">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="955ed-560">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-560">Az.OperationalInsights</span></span>
* <span data-ttu-id="955ed-561">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="955ed-561">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="955ed-562">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="955ed-562">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="955ed-563">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="955ed-563">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="955ed-564">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-564">Az.Resources</span></span>
* <span data-ttu-id="955ed-565">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="955ed-565">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="955ed-566">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="955ed-566">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="955ed-567">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="955ed-567">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="955ed-568">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="955ed-568">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-569">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-569">Az.Sql</span></span>
* <span data-ttu-id="955ed-570">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="955ed-570">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="955ed-571">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="955ed-571">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-572">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-572">Az.Websites</span></span>
* <span data-ttu-id="955ed-573">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="955ed-573">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="955ed-574">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-574">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-575">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-575">Az.Accounts</span></span>
* <span data-ttu-id="955ed-576">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="955ed-576">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="955ed-577">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="955ed-577">Az.AnalysisServices</span></span>
<span data-ttu-id="955ed-578">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="955ed-578">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-579">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-579">Az.Compute</span></span>
* <span data-ttu-id="955ed-580">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="955ed-580">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="955ed-581">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="955ed-581">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="955ed-582">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="955ed-582">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-583">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-583">Az.RecoveryServices</span></span>
<span data-ttu-id="955ed-584">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="955ed-584">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-585">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-585">Az.Resources</span></span>
* <span data-ttu-id="955ed-586">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="955ed-586">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="955ed-587">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="955ed-587">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="955ed-588">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="955ed-588">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="955ed-589">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="955ed-589">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-590">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-590">Az.Sql</span></span>
* <span data-ttu-id="955ed-591">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="955ed-591">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="955ed-592">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="955ed-592">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="955ed-593">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="955ed-593">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="955ed-594">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-594">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-595">Az.Accounts</span></span>
* <span data-ttu-id="955ed-596">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="955ed-596">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="955ed-597">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="955ed-597">Az.AnalysisServices</span></span>
* <span data-ttu-id="955ed-598">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="955ed-598">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-599">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-599">Az.RecoveryServices</span></span>
* <span data-ttu-id="955ed-600">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="955ed-600">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="955ed-601">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-601">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-602">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-602">Az.Accounts</span></span>
* <span data-ttu-id="955ed-603">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="955ed-603">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="955ed-604">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-604">Update incorrect online help URLs</span></span>
* <span data-ttu-id="955ed-605">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="955ed-605">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="955ed-606">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="955ed-606">Az.Aks</span></span>
* <span data-ttu-id="955ed-607">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-607">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="955ed-608">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-608">Az.Automation</span></span>
* <span data-ttu-id="955ed-609">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="955ed-609">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="955ed-610">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-610">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="955ed-611">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="955ed-611">Az.Cdn</span></span>
* <span data-ttu-id="955ed-612">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-612">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-613">Az.Compute</span></span>
* <span data-ttu-id="955ed-614">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="955ed-614">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="955ed-615">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="955ed-615">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="955ed-616">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="955ed-616">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="955ed-617">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="955ed-617">Az.ContainerRegistry</span></span>
* <span data-ttu-id="955ed-618">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-618">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="955ed-619">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="955ed-619">Az.DataFactory</span></span>
* <span data-ttu-id="955ed-620">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="955ed-620">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-621">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-621">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-622">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="955ed-622">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="955ed-623">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="955ed-623">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="955ed-624">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-624">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="955ed-625">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="955ed-625">Az.IotHub</span></span>
* <span data-ttu-id="955ed-626">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="955ed-626">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="955ed-627">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-627">Az.KeyVault</span></span>
* <span data-ttu-id="955ed-628">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-628">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-629">Az.Network</span></span>
* <span data-ttu-id="955ed-630">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-630">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-631">Az.Resources</span></span>
* <span data-ttu-id="955ed-632">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="955ed-632">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="955ed-633">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="955ed-633">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="955ed-634">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="955ed-634">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="955ed-635">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="955ed-635">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="955ed-636">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="955ed-636">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="955ed-637">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="955ed-637">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="955ed-638">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="955ed-638">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="955ed-639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="955ed-639">Az.ServiceFabric</span></span>
* <span data-ttu-id="955ed-640">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="955ed-640">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="955ed-641">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="955ed-641">Fix some error messages.</span></span>
* <span data-ttu-id="955ed-642">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="955ed-642">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="955ed-643">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="955ed-643">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="955ed-644">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="955ed-644">Az.SignalR</span></span>
* <span data-ttu-id="955ed-645">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-645">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-646">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-646">Az.Sql</span></span>
* <span data-ttu-id="955ed-647">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-647">Update incorrect online help URLs</span></span>
* <span data-ttu-id="955ed-648">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="955ed-648">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="955ed-649">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="955ed-649">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="955ed-650">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="955ed-650">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-651">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-651">Az.Storage</span></span>
* <span data-ttu-id="955ed-652">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="955ed-653">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="955ed-653">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="955ed-654">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="955ed-654">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="955ed-655">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="955ed-655">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="955ed-656">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="955ed-656">Az.TrafficManager</span></span>
* <span data-ttu-id="955ed-657">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-657">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-658">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-658">Az.Websites</span></span>
* <span data-ttu-id="955ed-659">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="955ed-659">Update incorrect online help URLs</span></span>
* <span data-ttu-id="955ed-660">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="955ed-660">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="955ed-661">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="955ed-661">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="955ed-662">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="955ed-662">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="955ed-663">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-663">Az.Accounts</span></span>
* <span data-ttu-id="955ed-664">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="955ed-664">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-665">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-665">Az.Compute</span></span>
* <span data-ttu-id="955ed-666">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="955ed-666">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="955ed-667">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="955ed-667">Updated the description of ID in help files</span></span>
* <span data-ttu-id="955ed-668">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-668">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-669">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-669">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-670">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="955ed-670">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="955ed-671">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="955ed-671">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="955ed-672">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="955ed-672">Az.EventGrid</span></span>
* <span data-ttu-id="955ed-673">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="955ed-673">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="955ed-674">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="955ed-674">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="955ed-675">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="955ed-675">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="955ed-676">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="955ed-676">Event Time-To-Live,</span></span>
        - <span data-ttu-id="955ed-677">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="955ed-677">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="955ed-678">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="955ed-678">Dead letter endpoint.</span></span>
    - <span data-ttu-id="955ed-679">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="955ed-679">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="955ed-680">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="955ed-680">Event Time-To-Live,</span></span>
        - <span data-ttu-id="955ed-681">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="955ed-681">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="955ed-682">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="955ed-682">Dead letter endpoint.</span></span>
* <span data-ttu-id="955ed-683">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="955ed-683">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="955ed-684">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="955ed-684">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="955ed-685">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="955ed-685">Az.IotHub</span></span>
* <span data-ttu-id="955ed-686">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="955ed-686">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="955ed-687">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="955ed-687">Az.LogicApp</span></span>
* <span data-ttu-id="955ed-688">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="955ed-688">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-689">Az.Resources</span></span>
* <span data-ttu-id="955ed-690">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="955ed-690">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="955ed-691">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="955ed-691">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="955ed-692">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="955ed-692">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="955ed-693">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="955ed-693">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="955ed-694">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="955ed-694">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="955ed-695">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="955ed-695">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="955ed-696">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="955ed-696">Az.SignalR</span></span>
* <span data-ttu-id="955ed-697">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-697">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-698">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-698">Az.Sql</span></span>
* <span data-ttu-id="955ed-699">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="955ed-699">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="955ed-700">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-700">Az.Storage</span></span>
* <span data-ttu-id="955ed-701">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="955ed-701">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="955ed-702">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="955ed-702">New-AzStorageContext</span></span>
* <span data-ttu-id="955ed-703">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="955ed-703">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="955ed-704">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="955ed-704">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-705">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-705">Az.Websites</span></span>
* <span data-ttu-id="955ed-706">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="955ed-706">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="955ed-707">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-707">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="955ed-708">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-708">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="955ed-709">Geral</span><span class="sxs-lookup"><span data-stu-id="955ed-709">General</span></span>

- <span data-ttu-id="955ed-710">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="955ed-710">General Availability of Az Module</span></span>
- <span data-ttu-id="955ed-711">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="955ed-711">Online help for each module</span></span>
- <span data-ttu-id="955ed-712">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="955ed-712">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="955ed-713">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="955ed-713">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="955ed-714">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-714">Az.Accounts</span></span>
- <span data-ttu-id="955ed-715">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="955ed-715">Changed from Az.Profile</span></span>
- <span data-ttu-id="955ed-716">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="955ed-716">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="955ed-717">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="955ed-717">Az.ApiManagement</span></span>
- <span data-ttu-id="955ed-718">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="955ed-718">Fixes for #7002</span></span>
- <span data-ttu-id="955ed-719">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-719">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="955ed-720">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="955ed-720">Az.Batch</span></span>
- <span data-ttu-id="955ed-721">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="955ed-721">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="955ed-722">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="955ed-722">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="955ed-723">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-723">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="955ed-724">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="955ed-724">Az.Billing</span></span>
- <span data-ttu-id="955ed-725">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-725">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="955ed-726">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="955ed-726">Az.CognitivServices</span></span>
- <span data-ttu-id="955ed-727">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-727">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="955ed-728">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="955ed-728">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="955ed-729">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-729">Az.ContainerInstance</span></span>
- <span data-ttu-id="955ed-730">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="955ed-730">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="955ed-731">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="955ed-731">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="955ed-732">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-732">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="955ed-733">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-733">Az.DataLakeStore</span></span>
- <span data-ttu-id="955ed-734">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-734">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="955ed-735">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="955ed-735">Az.Monitor</span></span>
- <span data-ttu-id="955ed-736">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-736">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="955ed-737">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="955ed-737">Az.KeyVault</span></span>
- <span data-ttu-id="955ed-738">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="955ed-738">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="955ed-739">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="955ed-739">Az.MachineLearning</span></span>
- <span data-ttu-id="955ed-740">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="955ed-740">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="955ed-741">Az.Media</span><span class="sxs-lookup"><span data-stu-id="955ed-741">Az.Media</span></span>
- <span data-ttu-id="955ed-742">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="955ed-742">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="955ed-743">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-743">Az.Network</span></span>
<span data-ttu-id="955ed-744">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="955ed-744">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="955ed-745">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="955ed-745">New cmdlets added:</span></span>
        - <span data-ttu-id="955ed-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-748">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-748">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-751">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="955ed-751">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="955ed-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="955ed-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="955ed-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="955ed-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="955ed-754">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="955ed-754">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="955ed-755">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="955ed-755">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="955ed-756">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="955ed-756">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="955ed-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="955ed-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="955ed-758">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-758">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="955ed-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="955ed-760">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="955ed-760">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="955ed-761">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="955ed-761">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="955ed-762">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="955ed-762">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="955ed-763">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="955ed-763">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="955ed-764">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="955ed-764">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="955ed-765">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="955ed-765">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="955ed-766">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-766">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="955ed-767">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-767">Az.OperationalInsights</span></span>
- <span data-ttu-id="955ed-768">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-768">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="955ed-769">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="955ed-769">Az.Profile</span></span>
- <span data-ttu-id="955ed-770">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="955ed-770">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-771">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-771">Az.RecoveryServices</span></span>
- <span data-ttu-id="955ed-772">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-772">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="955ed-773">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-773">Az.Resources</span></span>
- <span data-ttu-id="955ed-774">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-774">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="955ed-775">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="955ed-775">Az.ServiceFabric</span></span>
- <span data-ttu-id="955ed-776">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="955ed-776">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="955ed-777">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-777">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="955ed-778">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="955ed-778">Az.SIgnalR</span></span>
- <span data-ttu-id="955ed-779">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="955ed-779">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="955ed-780">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-780">Az.Sql</span></span>
- <span data-ttu-id="955ed-781">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="955ed-781">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="955ed-782">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="955ed-782">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="955ed-783">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-783">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="955ed-784">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-784">Az.Storage</span></span>
- <span data-ttu-id="955ed-785">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-785">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="955ed-786">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-786">Az.Websites</span></span>
- <span data-ttu-id="955ed-787">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="955ed-787">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="955ed-788">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-788">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="955ed-789">Geral</span><span class="sxs-lookup"><span data-stu-id="955ed-789">General</span></span>

* <span data-ttu-id="955ed-790">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="955ed-790">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="955ed-791">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-791">Az.Compute</span></span>

* <span data-ttu-id="955ed-792">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="955ed-792">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="955ed-793">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-793">Az.DataLakeStore</span></span>

* <span data-ttu-id="955ed-794">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="955ed-794">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="955ed-795">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="955ed-795">Az.FrontDoor</span></span>

* <span data-ttu-id="955ed-796">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="955ed-796">Fixed some broken links</span></span>
    - <span data-ttu-id="955ed-797">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="955ed-797">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="955ed-798">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="955ed-798">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="955ed-799">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="955ed-799">Az.RecoveryServices</span></span>

* <span data-ttu-id="955ed-800">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="955ed-800">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="955ed-801">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="955ed-801">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="955ed-802">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-802">Az.Resources</span></span>

* <span data-ttu-id="955ed-803">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="955ed-803">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="955ed-804">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="955ed-804">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="955ed-805">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-805">Az.Sql</span></span>

* <span data-ttu-id="955ed-806">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="955ed-806">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="955ed-807">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="955ed-807">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="955ed-808">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="955ed-808">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="955ed-809">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-809">Az.Storage</span></span>

* <span data-ttu-id="955ed-810">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="955ed-810">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="955ed-811">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="955ed-811">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="955ed-812">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="955ed-812">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="955ed-813">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="955ed-813">Support Static Website configuration</span></span>
    - <span data-ttu-id="955ed-814">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="955ed-814">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="955ed-815">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="955ed-815">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="955ed-816">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-816">Az.Websites</span></span>

* <span data-ttu-id="955ed-817">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="955ed-817">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="955ed-818">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="955ed-818">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="955ed-819">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="955ed-819">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="955ed-820">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-820">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="955ed-821">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="955ed-821">Az.ApiManagement</span></span>
* <span data-ttu-id="955ed-822">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="955ed-822">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="955ed-823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="955ed-823">Az.Automation</span></span>
* <span data-ttu-id="955ed-824">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="955ed-824">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="955ed-825">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="955ed-825">Added Update Management cmdlets</span></span>
* <span data-ttu-id="955ed-826">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="955ed-826">Added Source Control cmdlets</span></span>
* <span data-ttu-id="955ed-827">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="955ed-827">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="955ed-828">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="955ed-828">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="955ed-829">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-829">Az.Compute</span></span>
* <span data-ttu-id="955ed-830">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="955ed-830">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="955ed-831">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="955ed-831">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="955ed-832">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-832">Az.ContainerInstance</span></span>
* <span data-ttu-id="955ed-833">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="955ed-833">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="955ed-834">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="955ed-834">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="955ed-835">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="955ed-835">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="955ed-836">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-836">Az.Network</span></span>
* <span data-ttu-id="955ed-837">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="955ed-837">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="955ed-838">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="955ed-838">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="955ed-839">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="955ed-839">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="955ed-840">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="955ed-840">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="955ed-841">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="955ed-841">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="955ed-842">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="955ed-842">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="955ed-843">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="955ed-843">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="955ed-844">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="955ed-844">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="955ed-845">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="955ed-845">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="955ed-846">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="955ed-846">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="955ed-847">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="955ed-847">Az.Relay</span></span>
* <span data-ttu-id="955ed-848">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="955ed-848">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="955ed-849">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-849">Az.Resources</span></span>
* <span data-ttu-id="955ed-850">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="955ed-850">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="955ed-851">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="955ed-851">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="955ed-852">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="955ed-852">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="955ed-853">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="955ed-853">Az.ServiceFabric</span></span>
* <span data-ttu-id="955ed-854">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="955ed-854">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="955ed-855">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-855">Az.Sql</span></span>
* <span data-ttu-id="955ed-856">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-856">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="955ed-857">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-857">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="955ed-858">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-858">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="955ed-859">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-859">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="955ed-860">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="955ed-860">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="955ed-861">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="955ed-861">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="955ed-862">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="955ed-862">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="955ed-863">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="955ed-863">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="955ed-864">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="955ed-864">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="955ed-865">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="955ed-865">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="955ed-866">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="955ed-866">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="955ed-867">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="955ed-867">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="955ed-868">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="955ed-868">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="955ed-869">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="955ed-869">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="955ed-870">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="955ed-870">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="955ed-871">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="955ed-871">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="955ed-872">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="955ed-872">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="955ed-873">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-873">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="955ed-874">Geral</span><span class="sxs-lookup"><span data-stu-id="955ed-874">General</span></span>
* <span data-ttu-id="955ed-875">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="955ed-875">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="955ed-876">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="955ed-876">Az.Profile</span></span>
* <span data-ttu-id="955ed-877">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="955ed-877">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="955ed-878">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="955ed-878">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="955ed-879">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="955ed-879">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="955ed-880">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="955ed-880">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="955ed-881">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="955ed-881">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="955ed-882">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="955ed-882">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="955ed-883">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="955ed-883">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="955ed-884">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="955ed-884">Az.CognitiveServices</span></span>
* <span data-ttu-id="955ed-885">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="955ed-885">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-886">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-886">Az.Compute</span></span>
* <span data-ttu-id="955ed-887">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="955ed-887">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="955ed-888">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="955ed-888">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="955ed-889">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="955ed-889">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-890">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-890">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-891">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="955ed-891">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="955ed-892">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="955ed-892">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="955ed-893">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="955ed-893">Az.Insights</span></span>
* <span data-ttu-id="955ed-894">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="955ed-894">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="955ed-895">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="955ed-895">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="955ed-896">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="955ed-896">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="955ed-897">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="955ed-897">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-898">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-898">Az.Network</span></span>
* <span data-ttu-id="955ed-899">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="955ed-899">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="955ed-900">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="955ed-900">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="955ed-901">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="955ed-901">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="955ed-902">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="955ed-902">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="955ed-903">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="955ed-903">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="955ed-904">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="955ed-904">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="955ed-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="955ed-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="955ed-906">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="955ed-906">Az.PolicyInsights</span></span>
* <span data-ttu-id="955ed-907">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="955ed-907">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-908">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-908">Az.Resources</span></span>
* <span data-ttu-id="955ed-909">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="955ed-909">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="955ed-910">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="955ed-910">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="955ed-911">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="955ed-911">Az.ServiceBus</span></span>
* <span data-ttu-id="955ed-912">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="955ed-912">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="955ed-913">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="955ed-913">Az.ServiceFabric</span></span>
* <span data-ttu-id="955ed-914">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="955ed-914">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="955ed-915">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="955ed-915">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="955ed-916">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="955ed-916">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="955ed-917">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="955ed-917">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="955ed-918">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="955ed-918">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="955ed-919">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-919">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="955ed-920">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="955ed-920">Az.Profile</span></span>
* <span data-ttu-id="955ed-921">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="955ed-921">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="955ed-922">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="955ed-922">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-923">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-923">Az.Compute</span></span>
* <span data-ttu-id="955ed-924">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="955ed-924">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="955ed-925">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="955ed-925">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="955ed-926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="955ed-926">Az.DataLakeStore</span></span>
* <span data-ttu-id="955ed-927">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="955ed-927">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="955ed-928">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="955ed-928">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="955ed-929">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="955ed-929">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="955ed-930">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="955ed-930">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="955ed-931">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="955ed-931">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-932">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-932">Az.Network</span></span>
* <span data-ttu-id="955ed-933">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="955ed-933">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="955ed-934">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="955ed-934">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-935">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-935">Az.Resources</span></span>
* <span data-ttu-id="955ed-936">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="955ed-936">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="955ed-937">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="955ed-937">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="955ed-938">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-938">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="955ed-939">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="955ed-939">Azure.Storage</span></span>
* <span data-ttu-id="955ed-940">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="955ed-940">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="955ed-941">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="955ed-941">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="955ed-942">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="955ed-942">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="955ed-943">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="955ed-943">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="955ed-944">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="955ed-944">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="955ed-945">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="955ed-945">Az.CognitiveServices</span></span>
* <span data-ttu-id="955ed-946">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="955ed-946">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="955ed-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="955ed-947">Az.Compute</span></span>
* <span data-ttu-id="955ed-948">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="955ed-948">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="955ed-949">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="955ed-949">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="955ed-950">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="955ed-950">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="955ed-951">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="955ed-951">Az.DataFactoryV2</span></span>
* <span data-ttu-id="955ed-952">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="955ed-952">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="955ed-953">Az.Network</span><span class="sxs-lookup"><span data-stu-id="955ed-953">Az.Network</span></span>
* <span data-ttu-id="955ed-954">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="955ed-954">Added NetworkProfile functionality.</span></span> <span data-ttu-id="955ed-955">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="955ed-955">new cmdlets added</span></span>
    - <span data-ttu-id="955ed-956">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="955ed-956">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="955ed-957">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="955ed-957">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="955ed-958">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="955ed-958">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="955ed-959">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="955ed-959">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="955ed-960">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-960">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="955ed-961">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-961">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="955ed-962">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="955ed-962">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="955ed-963">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="955ed-963">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="955ed-964">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="955ed-964">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="955ed-965">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="955ed-965">Az.RedisCache</span></span>
* <span data-ttu-id="955ed-966">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="955ed-966">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="955ed-967">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="955ed-967">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="955ed-968">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="955ed-968">Az.Resources</span></span>
* <span data-ttu-id="955ed-969">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="955ed-969">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="955ed-970">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="955ed-970">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="955ed-971">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="955ed-971">Az.Sql</span></span>
* <span data-ttu-id="955ed-972">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="955ed-972">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="955ed-973">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="955ed-973">Az.Websites</span></span>
* <span data-ttu-id="955ed-974">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="955ed-974">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="955ed-975">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="955ed-975">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="955ed-976">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="955ed-976">0.2.0 - September 2018</span></span>
 <span data-ttu-id="955ed-977">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="955ed-977">Initial Release</span></span>