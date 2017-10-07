Instalador do Azure PowerShell 4.3.1: [ligação](https://github.com/Azure/azure-powershell/releases/download/v4.3.1-August2017/azure-powershell.4.3.1.msi)

Módulo da Galeria para Cmdlets ARM: [ligação](https://www.powershellgallery.com/packages/AzureRM/4.3.1)

Módulo da Galeria para Cmdlets Legados para a Gestão de Serviços (RDFE): [ligação](https://www.powershellgallery.com/packages/Azure/4.3.1)

## <a name="changes-in-431"></a>Alterações na versão 4.3.1

- Corrigido o problema em que determinadas assemblagens não eram assinadas, o que resultava num erro `could not load file or assembly` quando se importavam módulos

## <a name="changes-in-430"></a>Alterações na versão 4.3.0

* AnalysisServices
    * Erro corrigido em Set-AzureRmAnalysisServciesServer
        - Quando o administrador não é fornecido, o mesmo será removido.
    * BackupBlobContainerUri adicionado em New-AzureRmAnalysisServicesServer e Set-AzureRmAnalysisServicesServer
        - Pode definir/desativar o contentor de blobs de cópia de segurança para fazer a cópia de segurança ou o restauro do Servidor do Azure Analysis Services
    * Pesquisa de SKU atualizada em New-AzureRmAnalysisServicesServer e Set-AzureRmAnalysisServicesServer
        - SKU hard-coded alterado para pesquisa dinâmica.
    * Add-AzureAnalysisServicesAccount para suportar o início de sessão com o Principal de Serviço
* Automatização
    * Alterações aos cmdlets AutomationDSC* para extrair mais do que 100 registos
    * Resolvido o problema em que os fluxos Verbosos paravam de funcionar depois de chamar alguns cmdlets da Automatização (por exemplo, Get-AzureRmAutomationVariable, Get-AzureRmAutomationJob).
    * Adicionado o suporte para o controlo de versões da Compilação NodeConfiguration em StartAzureAutomationDscCompilationJob e ImportAzureAutomationDscNodeConfiguration.
    * Correções de erros existentes - A correção do problema de alias é #3775 e do alias runOn e do suporte para HybridWorkers.
* Computação
    * Set-AzureRmVMAEMExtension: adiciona suporte para novos tamanhos de Disco Premium
    * Set-AzureRmVMAEMExtension: adiciona suporte para a série M
    * Adicionado o parâmetro ForceUpdateTag a Add-AzureRmVmssExtension
    * Adicionado o parâmetro Principal a New-AzureRmVmssIpConfig
    * Adicionado o parâmetro EnableAcceleratedNetworking a Add-AzureRmVmssNetworkInterfaceConfig
    * Adicionado o InstanceId a Set-AzureRmVmss
    * Exposição de MaintenanceRedeployStatus a Get-AzureRmVM -Saída do estado
    * Exposição da Restrição e Capacidade ao formato de tabela de Get-AzureRmComputeResourceSku
* DataLakeStore
    * Correção do problema: https://github.com/Azure/azure-powershell/issues/4323
* EventHub
    * Adicionada a propriedade ResourceGroup a NamespaceAttributes
        - “ResourceGroup” obtém o nome do grupo de recursos em que se encontra o Espaço de Nomes
    * Atualizados os commandlets com um novo parâmetro e alias de parâmetro
        - Atualizados os cmdlets abaixo com ParameterSets para o Espaço de Nomes e EventHub para o funcionamento de AuthorizationRule
        - New-AzureRmEventHubAuthorizationRule
            + Adiciona uma nova AuthorizationRule ao Espaço de Nomes ou EventHub existentes.
        - Get-AzureRmEventHubAuthorizationRule
            + Obtém a AuthorizationRule/Lista de AuthorizationRules do Espaço de Nomes ou EventHub existentes.
        - Set-AzureRmEventHubAuthorizationRule
            + Atualiza as propriedades da AuthorizationRule ou EventHub existentes.
        - Remove-AzureRmEventHubAuthorizationRule
            + Elimina a AuthorizationRule existente do Espaço de Nomes ou EventHub existentes.
        - New-AzureRmEventHubKey
            + Gera uma nova Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes ou EventHub existentes.
        - Get-AzureRmEventHubKey
            + Obtém a Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes ou EventHub existentes.
* Rede
    * New-AzureRmExpressRouteCircuitPeeringConfig: adicionado suporte para IPv6. Novo parâmetro opcional adicionado
        - PeerAddressType
    * Set-AzureRmExpressRouteCircuitPeeringConfig: adicionado suporte para IPv6. Novo parâmetro opcional adicionado
        - PeerAddressType
    * Remove-AzureRmExpressRouteCircuitPeeringConfig: adicionado suporte para IPv6. Novo parâmetro opcional adicionado
        - PeerAddressType
    * Parâmetro marcado -ProbeEnabled como obsoleto
        - Add-AzureRmApplicationGatewayBackendHttpSettings
        - New-AzureRmApplicationGatewayBackendHttpSettings
        - Set-AzureRmApplicationGatewayBackendHttpSettings
* Perfil
    * A recolha de dados foi ativada por predefinição. Os dados de utilização são recolhidos pela Microsoft para melhorar a experiência de utilizador. Os dados são anónimos e não incluem valores de argumento da linha de comandos.
        - Utilize o cmdlet Disable-AzureRmDataCollection para desativar a funcionalidade
        - Utilize o cmdlet Enable-AzureRmDataCollection para ativar a funcionalidade
* Recursos
    * Adicionado Suporte para a validação de âmbitos para os seguintes commandlets de roledefinition e roleassignment antes de enviar o pedido para o ARM
        - Get-AzureRMRoleAssignment
        - New-AzureRMRoleAssignment
        - Remove-AzureRMRoleAssignment
        - Get-AzureRMRoleDefinition
        - New-AzureRMRoleDefinition
        - Remove-AzureRMRoleDefinition
        - Set-AzureRMRoleDefinition
* ServiceBus
    * Adicionado abaixo novos commandlets para AuthorizationRules do Espaço de Nomes, Fila e Tópico. De acordo com o parâmetro definido, as operações da regra de autorização são realizadas.
     - New-AzureRmServiceBusAuthorizationRule
       - Adiciona uma nova AuthorizationRule ao Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Get-AzureRmServiceBusAuthorizationRule
       - Obtém a AuthorizationRule/Lista de AuthorizationRules do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Set-AzureRmServiceBusAuthorizationRule
       - Atualiza as propriedades da AuthorizationRule existente do Espaço de Nomes/Fila/Tópico do ServiceBus.
     - New-AzureRmServiceBusKey
       - Gera uma nova Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Get-AzureRmServiceBusKey
       - Obtém a Chave Primária/Secundária da AuthorizationRule do Espaço de Nomes/Fila/Tópico existente do ServiceBus.
     - Remove-AzureRmServiceBusNamespaceAuthorizationRule
       - Elimina a AuthorizationRule existente do Espaço de Nomes/Fila/Tópico do ServiceBus.
    * Adicionada a propriedade ResourceGroup a NamespaceAttributes
* SQL
    * Atualização de Set-AzureRmSqlServerTransparentDataEncryptionProtector para apresentar um aviso e pedir confirmação se o Tipo de Protetor de Encriptação estiver definido para AzureKeyVault
    * A adicionar novos cmdlets atualizados para as definições de Auditoria
        - A adicionar o cmdlet Get-AzureRmSqlDatabaseAuditing, o qual obtém as definições de auditoria de uma base de dados SQL do Azure.
        - A adicionar o cmdlet Get-AzureRmSqlServerAuditing, o qual obtém as definições de auditoria de um servidor SQL do Azure.
        - A adicionar o cmdlet Set-AzureRmSqlDatabaseAuditing, o qual altera as definições de auditoria de uma base de dados SQL do Azure.
        - A adicionar o cmdlet Set-AzureRmSqlServerAuditing, o qual altera as definições de auditoria de um servidor SQL do Azure.
    * Descontinuar os cmdlets existentes da política de Auditoria
        - Descontinuar Get-AzureRmSqlDatabaseAuditingPolicy
        - Descontinuar Get-AzureRmSqlServerAuditingPolicy
        - Descontinuar Set-AzureRmSqlDatabaseAuditingPolicy
        - Descontinuar Set-AzureRmSqlServerAuditingPolicy
        - Descontinuar Use-AzureRmSqlServerAuditingPolicy
        - Descontinuar Remove-AzureRmSqlDatabaseAuditing
        - Descontinuar Remove-AzureRmSqlServerAuditing
    * A análise do ficheiro de esquema de Update-AzureRmSqlSyncGroup passa a ser não sensível às maiúsculas e minúsculas.
* Armazenamento
    * Adicionado suporte a NeworkRule para os cmdlets de conta de armazenamento do modo de recursos
        - New-AzureRmStorageAccount
        - Set-AzureRmStorageAccount
        - Get-AzureRmStorageAccountNetworkRuleSet
        - Update-AzureRmStorageAccountNetworkRuleSet
        - Add-AzureRmStorageAccountNetworkRule
        - Remove-AzureRmStorageAccountNetworkRule

Ver as [alterações desde a última versão](https://github.com/Azure/azure-powershell/compare/v4.2.1-July2017...v4.3.1-August2017)
