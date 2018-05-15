# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a><span data-ttu-id="dfb73-101">Alterações recentes ao Microsoft Azure PowerShell 3.0.0.</span><span class="sxs-lookup"><span data-stu-id="dfb73-101">Breaking changes for Microsoft Azure PowerShell 3.0.0.</span></span>

<span data-ttu-id="dfb73-102">Este documento é simultaneamente uma notificação das alterações recentes e um guia de migração para os consumidores de cmdlets do Microsoft Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dfb73-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span>  <span data-ttu-id="dfb73-103">Cada secção descreve não só o catalisador da alteração recente como o caminho de migração que envolve o menor esforço.</span><span class="sxs-lookup"><span data-stu-id="dfb73-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span>  <span data-ttu-id="dfb73-104">Para obter um contexto mais aprofundado, consulte o pedido detalhado associado a cada alteração.</span><span class="sxs-lookup"><span data-stu-id="dfb73-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="dfb73-105">Índice</span><span class="sxs-lookup"><span data-stu-id="dfb73-105">Table of Contents</span></span>
1. [<span data-ttu-id="dfb73-106">Alterações recentes aos cmdlets de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="dfb73-106">Breaking changes to Data Lake Store cmdlets</span></span>](#breaking-changes-to-data-lake-store-cmdlets)
2. [<span data-ttu-id="dfb73-107">Alterações recentes aos cmdlets de ApiManagement</span><span class="sxs-lookup"><span data-stu-id="dfb73-107">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
3. [<span data-ttu-id="dfb73-108">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="dfb73-108">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a><span data-ttu-id="dfb73-109">Alterações recentes aos cmdlets de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="dfb73-109">Breaking changes to Data Lake Store cmdlets</span></span>

<span data-ttu-id="dfb73-110">Os seguintes cmdlets foram afetados nesta versão ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)):</span><span class="sxs-lookup"><span data-stu-id="dfb73-110">The following cmdlets were affected this release ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)):</span></span>

<span data-ttu-id="dfb73-111">**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**</span><span class="sxs-lookup"><span data-stu-id="dfb73-111">**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**</span></span>
- <span data-ttu-id="dfb73-112">Este cmdlet foi removido e substituído por ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span><span class="sxs-lookup"><span data-stu-id="dfb73-112">This cmdlet was removed and replaced with ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>
- <span data-ttu-id="dfb73-113">O cmdlet antigo devolvia um objeto complexo que representava a lista de controlo de acesso (ACL).</span><span class="sxs-lookup"><span data-stu-id="dfb73-113">The old cmdlet returned a complex object representing the access control list (ACL).</span></span> <span data-ttu-id="dfb73-114">O novo cmdlet devolve uma lista simples de entradas na ACL do caminho escolhido.</span><span class="sxs-lookup"><span data-stu-id="dfb73-114">The new cmdlet returns a simple list of entries in the chosen path's ACL.</span></span>

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="dfb73-115">**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="dfb73-115">**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="dfb73-116">Este cmdlet substitui o cmdlet antigo ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``.</span><span class="sxs-lookup"><span data-stu-id="dfb73-116">This cmdlet replaces the old cmdlet ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``.</span></span>
- <span data-ttu-id="dfb73-117">O novo cmdlet devolve uma lista simples de entradas na ACL do caminho escolhido, com o tipo ``DataLakeStoreItemAce[]``.</span><span class="sxs-lookup"><span data-stu-id="dfb73-117">This new cmdlet returns a simple list of entries in the chosen path's ACL, with type ``DataLakeStoreItemAce[]``.</span></span>
- <span data-ttu-id="dfb73-118">A saída deste cmdlet pode ser transmitida para o parâmetro ``-Acl`` dos seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="dfb73-118">The output of this cmdlet can be passed in to the ``-Acl`` parameter of the following cmdlets:</span></span>
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="dfb73-119">**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="dfb73-119">**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="dfb73-120">Agora, estes cmdlets aceitam ``DataLakeStoreItemAce[]`` para o parâmetro ``-Acl``.</span><span class="sxs-lookup"><span data-stu-id="dfb73-120">These cmdlets now accept ``DataLakeStoreItemAce[]`` for the ``-Acl`` parameter.</span></span>
- <span data-ttu-id="dfb73-121">``DataLakeStoreItemAce[]`` é devolvido por ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span><span class="sxs-lookup"><span data-stu-id="dfb73-121">``DataLakeStoreItemAce[]`` is returned by ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="dfb73-122">Alterações recentes aos cmdlets de ApiManagement</span><span class="sxs-lookup"><span data-stu-id="dfb73-122">Breaking changes to ApiManagement cmdlets</span></span>

<span data-ttu-id="dfb73-123">Os seguintes cmdlets foram afetados nesta versão ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)):</span><span class="sxs-lookup"><span data-stu-id="dfb73-123">The following cmdlets were affected this release ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)):</span></span>

<span data-ttu-id="dfb73-124">**New-AzureRmApiManagementVirtualNetwork**</span><span class="sxs-lookup"><span data-stu-id="dfb73-124">**New-AzureRmApiManagementVirtualNetwork**</span></span>
- <span data-ttu-id="dfb73-125">Os parâmetros necessários para fazer referência a uma rede virtual foram alterados: em vez de SubnetName e VnetId necessitam agora de SubnetResourceId no formato ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}``</span><span class="sxs-lookup"><span data-stu-id="dfb73-125">The required parameters to reference a virtual network changed from requiring SubnetName and VnetId to SubnetResourceId in format ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}``</span></span>

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

<span data-ttu-id="dfb73-126">**Preterição do cmdlet Set-AzureRmApiManagementVirtualNetworks**</span><span class="sxs-lookup"><span data-stu-id="dfb73-126">**Deprecating Cmdlet Set-AzureRmApiManagementVirtualNetworks**</span></span>
- <span data-ttu-id="dfb73-127">A preterição deste cmdlet surge na medida em que havia mais do que uma forma de definir a Rede Virtual associada à implementação de ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="dfb73-127">The Cmdlet is getting deprecated as there was more than one way to Set Virtual Network associated to ApiManagement deployment.</span></span>

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="dfb73-128">Alterações recentes aos cmdlets de Rede</span><span class="sxs-lookup"><span data-stu-id="dfb73-128">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="dfb73-129">Os seguintes cmdlets foram afetados nesta versão ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)):</span><span class="sxs-lookup"><span data-stu-id="dfb73-129">The following cmdlets were affected this release ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)):</span></span>

<span data-ttu-id="dfb73-130">**New-AzureRmVirtualNetworkGateway**</span><span class="sxs-lookup"><span data-stu-id="dfb73-130">**New-AzureRmVirtualNetworkGateway**</span></span>
- <span data-ttu-id="dfb73-131">A descrição das alterações efetuadas ``:- Bool parameter:-ActiveActive`` foi removida e ``SwitchParameter:-EnableActiveActiveFeature`` foi adicionado para ativar a funcionalidade Active-Active no gateway de rede virtual recém-criado.</span><span class="sxs-lookup"><span data-stu-id="dfb73-131">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and ``SwitchParameter:-EnableActiveActiveFeature`` is added for enabling Active-Active feature on newly creating virtual network gateway.</span></span>

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

<span data-ttu-id="dfb73-132">Set-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="dfb73-132">Set-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="dfb73-133">A descrição das alterações efetuadas ``:- Bool parameter:-ActiveActive`` foi removida e foram adicionados 2 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` para ativar e desativar a funcionalidade Active-Active no gateway de rede virtual.</span><span class="sxs-lookup"><span data-stu-id="dfb73-133">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and 2 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` are added for enabling and disabling Active-Active feature on virtual network gateway.</span></span>

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