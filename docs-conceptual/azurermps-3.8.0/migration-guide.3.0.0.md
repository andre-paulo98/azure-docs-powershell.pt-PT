# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a>Alterações recentes ao Microsoft Azure PowerShell 3.0.0.

Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.  Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.  Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.

## <a name="table-of-contents"></a>Índice
1. [Alterações recentes aos cmdlets de Data Lake Store](#breaking-changes-to-data-lake-store-cmdlets)
2. [Alterações recentes aos cmdlets de ApiManagement](#breaking-changes-to-apimanagement-cmdlets)
3. [Alterações recentes aos cmdlets de Rede](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a>Alterações recentes aos cmdlets de Data Lake Store

Os seguintes cmdlets foram afetados nesta versão ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)):

**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**
- Este cmdlet foi removido e substituído por ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.
- O cmdlet antigo devolvia um objeto complexo que representava a lista de controlo de acesso (ACL). O novo cmdlet devolve uma lista simples de entradas na ACL do caminho escolhido.

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**
- Este cmdlet substitui o cmdlet antigo ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``.
- O novo cmdlet devolve uma lista simples de entradas na ACL do caminho escolhido, com o tipo ``DataLakeStoreItemAce[]``.
- A saída deste cmdlet pode ser transmitida para o parâmetro ``-Acl`` dos seguintes cmdlets:
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**
- Agora, estes cmdlets aceitam ``DataLakeStoreItemAce[]`` para o parâmetro ``-Acl``.
- ``DataLakeStoreItemAce[]`` é devolvido por ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a>Alterações recentes aos cmdlets de ApiManagement

Os seguintes cmdlets foram afetados nesta versão ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)):

**New-AzureRmApiManagementVirtualNetwork**
- Os parâmetros necessários para fazer referência a uma rede virtual foram alterados: em vez de SubnetName e VnetId necessitam agora de SubnetResourceId no formato ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}``

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

**Preterição do cmdlet Set-AzureRmApiManagementVirtualNetworks**
- A preterição deste cmdlet surge na medida em que havia mais do que uma forma de definir a Rede Virtual associada à implementação de ApiManagement.

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a>Alterações recentes aos cmdlets de Rede

Os seguintes cmdlets foram afetados nesta versão ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)):

**New-AzureRmVirtualNetworkGateway**
- A descrição das alterações efetuadas ``:- Bool parameter:-ActiveActive`` foi removida e ``SwitchParameter:-EnableActiveActiveFeature`` foi adicionado para ativar a funcionalidade Active-Active no gateway de rede virtual recém-criado.

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

Set-AzureRmVirtualNetworkGateway
- A descrição das alterações efetuadas ``:- Bool parameter:-ActiveActive`` foi removida e foram adicionados 2 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` para ativar e desativar a funcionalidade Active-Active no gateway de rede virtual.

```powershell
# Old
# Sample of how the cmdlet was previously called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $true
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $false  

# New
# Sample of how the cmdlet should now be called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -EnableActiveActiveFeature
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -DisableActiveActiveFeature
```