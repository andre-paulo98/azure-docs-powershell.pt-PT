---
title: Introdução ao Azure PowerShell
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 10/30/2018
ms.openlocfilehash: 7367648a0a84cd5be5c7501ef4bf743a4290ce0f
ms.sourcegitcommit: 6685809f054203bd733c84f68acc69e53e5cca8c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982914"
---
# <a name="get-started-with-azure-powershell"></a>Introdução ao Azure PowerShell

O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager. Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou instalá-lo na máquina local. Este artigo ajuda-o a começar a utilizar o Azure PowerShell e explica os principais conceitos que lhe estão subjacentes.

## <a name="install-azure-powershell"></a>Instalar o Azure PowerShell

O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell. Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).

1. [Instalar o Azure PowerShell](install-az-ps.md).

2. Para verificar se a instalação foi concluída com êxito, execute `Get-InstalledModule Az -AllVersions` na sua linha de comandos.

## <a name="azure-cloud-shell"></a>Azure Cloud Shell

A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).

1. Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.

![Cloud Shell for PowerShell](~/media/get-started-azureps/cloud-powershell.png)

## <a name="sign-in-to-azure"></a>Iniciar sessão no Azure

Inicie sessão interativamente:

1. Digite `Connect-AzAccount`. O argumento `-Environment` permite-lhe autenticar-se numa região ou cloud diferente. Por exemplo, para se ligar ao Azure China:

    ```powershell-interactive
    Connect-AzAccount -Environment AzureChinaCloud
    ```

2. Obterá um token para utilizar em https://microsoft.com/devicelogin. Abra esta página no seu browser e introduza o token para iniciar sessão com as suas credenciais do Azure e autorizar o Azure PowerShell. 

Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição. Para saber mais sobre o processo de início de sessão e os métodos de autenticação disponíveis, veja [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md).

## <a name="create-a-windows-virtual-machine-using-simple-defaults"></a>Criar uma máquina virtual do Windows com predefinições simples

O cmdlet `New-AzVM` fornece uma sintaxe simplificada que facilita a criação de uma nova máquina virtual. Existem apenas dois valores de parâmetros que tem de fornecer: o nome da VM e um conjunto de credenciais para a conta de administrador local na VM.

Primeiro, crie o objeto de credencial.

```azurepowershell-interactive
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

```output
Windows PowerShell credential request.
Enter a username and password for the virtual machine.
User: localAdmin
Password for user localAdmin: *********
```

Em seguida, crie a VM.

```azurepowershell-interactive
New-AzVM -Name SampleVM -Credential $cred
```

```output
ResourceGroupName        : SampleVM
Id                       : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/SampleVM/providers/Microsoft.Compute/virtualMachines/SampleVM
VmId                     : 43f6275d-ce50-49c8-a831-5d5974006e63
Name                     : SampleVM
Type                     : Microsoft.Compute/virtualMachines
Location                 : eastus
Tags                     : {}
HardwareProfile          : {VmSize}
NetworkProfile           : {NetworkInterfaces}
OSProfile                : {ComputerName, AdminUsername, WindowsConfiguration, Secrets}
ProvisioningState        : Succeeded
StorageProfile           : {ImageReference, OsDisk, DataDisks}
FullyQualifiedDomainName : samplevm-2c0867.eastus.cloudapp.azure.com
```

Pode questionar-se sobre o que é criado e como a VM é configurada. Primeiro, vamos ver os nossos grupos de recursos.

```azurepowershell-interactive
Get-AzResourceGroup | Select-Object ResourceGroupName,Location
```

```output
ResourceGroupName          Location
-----------------          --------
cloud-shell-storage-westus westus
SampleVM                   eastus
```

É criado o grupo de recursos **cloud-shell-storage-westus** quando utilizar o Cloud Shell pela primeira vez. O grupo de recursos **SampleVM** foi criado pelo cmdlet `New-AzVM`.

Agora, que outros recursos foram criados neste novo grupo de recursos?

```azurepowershell-interactive
Get-AzResource |
  Where ResourceGroupName -eq SampleVM |
    Select-Object ResourceGroupName,Location,ResourceType,Name
```

```output
ResourceGroupName          Location ResourceType                            Name
-----------------          -------- ------------                            ----
SAMPLEVM                   eastus   Microsoft.Compute/disks                 SampleVM_OsDisk_1_9b286c54b168457fa1f8c47...
SampleVM                   eastus   Microsoft.Compute/virtualMachines       SampleVM
SampleVM                   eastus   Microsoft.Network/networkInterfaces     SampleVM
SampleVM                   eastus   Microsoft.Network/networkSecurityGroups SampleVM
SampleVM                   eastus   Microsoft.Network/publicIPAddresses     SampleVM
SampleVM                   eastus   Microsoft.Network/virtualNetworks       SampleVM
```

Vamos obter mais detalhes sobre a VM. Este exemplo mostra como obter informações sobre a Imagem do SO utilizada para criar a VM.

```azurepowershell-interactive
Get-AzVM -Name SampleVM -ResourceGroupName SampleVM |
  Select-Object -ExpandProperty StorageProfile |
    Select-Object -ExpandProperty ImageReference
```

```output
Publisher : MicrosoftWindowsServer
Offer     : WindowsServer
Sku       : 2016-Datacenter
Version   : latest
Id        :
```

## <a name="create-a-fully-configured-linux-virtual-machine"></a>Criar uma Máquina Virtual do Linux totalmente configurada

O exemplo anterior utilizou a sintaxe simplificada e os valores de parâmetros predefinidos para criar uma máquina virtual do Windows. Neste exemplo, fornecemos valores para todas as opções da máquina virtual.

### <a name="create-a-resource-group"></a>Criar um grupo de recursos

Neste exemplo, queremos criar um Grupo de Recursos. Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente. Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.

Vamos criar um grupo de recursos com o nome "MyResourceGroup" na região uswest2 do Azure. Para tal, escreva o comando seguinte:

```azurepowershell-interactive
New-AzResourceGroup -Name 'myResourceGroup' -Location 'westus2'
```

```output
ResourceGroupName : myResourceGroup
Location          : westus2
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

Este novo grupo de recursos será utilizado para conter todos os recursos necessários para a nova VM criada. Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos que são precisos e atribuí-los a uma configuração. Em seguida, podemos utilizar a configuração para criar a VM. Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório `.ssh` do seu perfil de utilizador.

#### <a name="create-the-required-network-resources"></a>Criar os recursos de rede necessários

Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual. Também podemos criar um endereço IP público para podermos ligar a esta VM. Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público. Por fim, criamos o NIC virtual através de todos os recursos anteriores.

```azurepowershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westus2"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString 'azurepassword' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-vm-configuration"></a>Criar a configuração da VM

Agora que temos os recursos necessários, podemos criar o objeto de configuração da VM.

```azurepowershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzVMConfig -VMName $vmName -VMSize Standard_B1s |
  Set-AzVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content -Raw "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"
```

### <a name="create-the-virtual-machine"></a>Criar a máquina virtual

Agora, podemos criar a VM com o respetivo objeto de configuração.

```azurepowershell-interactive
New-AzVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:

```powershell-interactive
ssh azureuser@$($publicIp.IpAddress)
```

```output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:../../..$
```

## <a name="creating-other-resources-in-azure"></a>Criar outros recursos no Azure

Acabámos de ver como são criados os Grupos de Recursos, as VMs do Linux e as VMs do Windows Server. Também pode criar muitos outros tipos de recursos do Azure.

Por exemplo, para criar um Balanceador de Carga da Rede do Azure que podemos, depois, associar às VMs acabadas de criar, podemos utilizar o comando de criação seguinte:

```azurepowershell-interactive
New-AzLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westus2
```

Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:

```azurepowershell-interactive
$subnetConfig = New-AzVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzVirtualNetwork -ResourceGroupName myResourceGroup -Location westus2 `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos. Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.

Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure. O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura. Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:

```azurepowershell-interactive
# Get a UUID for creating the apps to avoid name conflicts
$guid = [System.Guid]::NewGuid().ToString()

# Create an Azure AppService that we can host any number of web apps within
New-AzAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westus2

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzWebApp -Name MyWebApp-$guid -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westus2
New-AzWebApp -Name MyWebApp2-$guid -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westus2
```

## <a name="listing-deployed-resources"></a>Listar recursos implementados

Pode utilizar o cmdlet `Get-AzResource` para listar os recursos em execução no Azure. O exemplo seguinte mostra os recursos criados no novo grupo de recursos.

```azurepowershell-interactive
Get-AzResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westus2 Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westus2 Microsoft.Compute/disks
myLinuxVM                                             westus2 Microsoft.Compute/virtualMachines
myWindowsVM                                           westus2 Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westus2 Microsoft.Compute/virtualMachines/extensions
myNic1                                                westus2 Microsoft.Network/networkInterfaces
myNic2                                                westus2 Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westus2 Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westus2 Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westus2 Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westus2 Microsoft.Network/publicIPAddresses
MYvNET1                                               westus2 Microsoft.Network/virtualNetworks
MYvNET2                                               westus2 Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westus2 Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a>Eliminar recursos

Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo. Pode utilizar os cmdlets `Remove-Az*` para eliminar recursos de que já não precisa. Para remover a VM do Windows criada, utilize o seguinte comando:

```azurepowershell-interactive
Remove-AzVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

Ser-lhe-á pedido para confirmar se quer remover o recurso.

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

Também pode eliminar muitos recursos de uma só vez. Por exemplo, o comando seguinte elimina o grupo de recursos "MyResourceGroup" que utilizámos em todos os exemplos até agora.
Todos os recursos no grupo também são eliminados.

```azurepowershell-interactive
Remove-AzResourceGroup -Name myResourceGroup
```

```output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

A tarefa pode demorar vários minutos a concluir, consoante o número e o tipo de recursos.

## <a name="get-samples"></a>Obter exemplos

Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).

## <a name="next-steps"></a>Passos seguintes

* [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md)
* [Gerir subscrições do Azure com o Azure PowerShell](manage-subscriptions-azureps.md)
* [Criar principais de serviço no Azure com o Azure PowerShell](create-azure-service-principal-azureps.md)
* Obter ajuda da comunidade:
  * [Fórum do Azure no MSDN](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [Stackoverflow](http://go.microsoft.com/fwlink/?LinkId=320213)
