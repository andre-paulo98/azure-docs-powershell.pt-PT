---
title: Introdução ao Azure PowerShell | Microsoft Docs
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 7eb5e3fad31b5a92be1cfb36aefdaa7b920bae5f
ms.sourcegitcommit: 06f9206e025afa7207d4657c8f57c94ddb74817a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2018
ms.locfileid: "51211031"
---
# <a name="getting-started-with-azure-powershell"></a>Introdução ao Azure PowerShell

O Azure PowerShell foi concebido para gerir e administrar recursos do Azure a partir da linha de comandos e para criar scripts de automatização que funcionam no âmbito do Azure Resource Manager. Pode utilizá-lo no seu browser com o [Azure Cloud Shell](/azure/cloud-shell/overview) ou pode instalá-lo no seu computador local e utilizá-lo em qualquer sessão do PowerShell. Este artigo ajuda-o a começar a utilizá-lo e explica-lhe os conceitos principais subjacentes.

## <a name="connect"></a>Ligar

A forma mais simples de começar é [iniciar a Cloud Shell](/azure/cloud-shell/quickstart).

1. Inicie o Cloud Shell a partir do menu de navegação superior do portal do Azure.

   ![Ícone do Shell](~/media/get-started-azureps/shell-icon.png)

2. Selecione a subscrição que quer utilizar e crie uma conta de armazenamento.

   ![Criar uma conta de armazenamento](~/media/get-started-azureps/storage-prompt.png)

Assim que tiver sido criado o seu armazenamento, o Cloud Shell irá abrir uma sessão do PowerShell no browser.

![Cloud Shell para PowerShell](~/media/get-started-azureps/cloud-powershell.png)

Também pode instalar o Azure PowerShell e utilizá-lo localmente numa sessão do PowerShell.

## <a name="install-azure-powershell"></a>Instalar o Azure PowerShell

O primeiro passo é confirmar que tem instalada a versão mais recente do Azure PowerShell. Para obter informações sobre a versão mais recente, veja as [notas de versão](./release-notes-azureps.md).

1. [Instalar o Azure PowerShell](install-azurerm-ps.md).

2. Para verificar se a instalação foi concluída com êxito, execute `Get-Module AzureRM -ListAvailable` na sua linha de comandos.

## <a name="sign-in-to-azure"></a>Iniciar sessão no Azure

Inicie sessão interativamente:

1. Digite `Login-AzureRmAccount`. Obterá uma caixa de diálogo a solicitar as suas credenciais do Azure. A opção "-EnvironmentName" permite-lhe autenticar-se no Azure China ou Azure Alemanha.

   Por exemplo, Login-AzureRmAccount -EnvironmentName AzureChinaCloud

2. Escreva o endereço de e-mail e a palavra-passe associados à sua conta. O Azure autentica e guarda as informações das credenciais e, em seguida, fecha a janela.

Assim que tiver iniciado sessão numa conta do Azure, pode utilizar os cmdlets do Azure PowerShell para aceder e gerir os recursos na sua subscrição.

## <a name="create-a-resource-group"></a>Criar um grupo de recursos

Agora que já está tudo configurado, vamos utilizar o Azure PowerShell para criar recursos no Azure.

Comece por criar um Grupo de Recursos. Os Grupos de Recursos no Azure oferecem uma forma de gerir múltiplos recursos que quer agrupar logicamente. Por exemplo, pode criar um Grupo de Recursos para uma aplicação ou projeto e adicionar uma máquina virtual, uma base de dados e um serviço de CDN ao mesmo.

Vamos criar um grupo de recursos com o nome “MyResourceGroup" na região westeurope do Azure. Para tal, escreva o comando seguinte:

```powershell-interactive
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```Output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

## <a name="create-a-windows-virtual-machine"></a>Criar uma Máquina Virtual do Windows

Agora que temos o nosso grupo de recursos, vamos criar uma VM do Windows no mesmo. Para criar uma nova VM, temos de criar primeiro os outros recursos necessários e atribuí-los a uma configuração. Em seguida, podemos utilizar a configuração para criar a VM.

### <a name="create-the-required-network-resources"></a>Criar os recursos de rede necessários

Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual. Também podemos criar um endereço IP público para podermos ligar a esta VM. Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público. Por fim, criamos o NIC virtual através de todos os recursos anteriores.

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myWindowsVM"

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet1 -AddressPrefix 192.168.1.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET1 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 3389
$nsgRuleRDP = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleRDP  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 3389 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup1 -SecurityRules $nsgRuleRDP

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic1 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a>Criar a máquina virtual

Primeiro, é necessário um conjunto de credenciais para o sistema operativo.

```powershell-interactive
# Create user object
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

Agora que temos os recursos necessários, podemos criar a VM. Para este passo, criamos um objeto de configuração de VM e, em seguida, utilizamos a configuração para criar a VM.

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Windows -ComputerName $vmName -Credential $cred |
  Set-AzureRmVMSourceImage -PublisherName MicrosoftWindowsServer -Offer WindowsServer -Skus 2016-Datacenter -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

O comando `New-AzureRmVM` gera o resultado assim que a VM tiver sido totalmente criada e estiver pronta para ser utilizada.

```Output
RequestId IsSuccessStatusCode StatusCode ReasonPhrase
--------- ------------------- ---------- ------------
                         True         OK OK
```

Agora, inicie sessão na VM do Windows Server acabada de criar com o Ambiente de Trabalho Remoto e o endereço IP público da VM. O comando seguinte apresenta o endereço IP público criado no script anterior.

```powershell-interactive
$publicIp | Select-Object Name,IpAddress
```

```Output
Name                  IpAddress
----                  ---------
mypublicdns1400512543 xx.xx.xx.xx
```

Se estiver num sistema baseado no Windows, pode fazê-lo a partir da linha de comandos com o comando mstsc:

```powershell-interactive
mstsc /v:xx.xxx.xx.xxx
```

Indique a combinação de nome de utilizador/palavra-passe que utilizou quando criou a VM para iniciar sessão.

## <a name="create-a-linux-virtual-machine"></a>Criar uma Máquina Virtual do Linux

Para criar uma nova VM do Linux, temos de criar primeiro os outros recursos necessários e atribuí-los a uma configuração. Em seguida, podemos utilizar a configuração para criar a VM. Tal pressupõe que já criou o grupo de recursos, conforme mostrado anteriormente. Além disso, terá de ter uma chave pública SSH com o nome `id_rsa.pub` no diretório .ssh do seu perfil de utilizador.

### <a name="create-the-required-network-resources"></a>Criar os recursos de rede necessários

Primeiro, temos de criar uma configuração de sub-rede a utilizar no processo de criação da rede virtual. Também podemos criar um endereço IP público para podermos ligar a esta VM. Vamos criar um grupo de segurança de rede para proteger o acesso ao endereço público. Por fim, criamos o NIC virtual através de todos os recursos anteriores.

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString ' ' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a>Criar a máquina virtual

Agora que temos os recursos necessários, podemos criar a VM. Para este passo, criamos um objeto de configuração de VM e, em seguida, utilizamos a configuração para criar a VM.

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

Agora que a VM já está criada, pode iniciar sessão na sua nova VM do Linux através de SSH com o endereço IP público da VM que criou:

```bash
ssh xx.xxx.xxx.xxx
```

```Output
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

```powershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

Também podemos criar uma Rede Virtual privada nova (geralmente conhecida como “VNet” no Azure) para a nossa infraestrutura, utilizando o comando seguinte:

```powershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

O que torna o Azure e o Azure PowerShell poderosos é o facto de poderem ser utilizados não só para obter a infraestrutura baseada na cloud, como também para criar serviços de plataformas geridos. Os serviços de plataforma geridos podem, igualmente, ser combinados com a infraestrutura, para criar soluções ainda mais poderosas.

Por exemplo, pode utilizar o Azure PowerShell para criar um AppService do Azure. O AppService do Azure é um serviço de plataforma gerido que proporciona uma excelente forma de alojar aplicações Web sem que tenha de se preocupar com a infraestrutura. Depois de criar o AppService do Azure, pode criar duas novas Aplicações Web do Azure no AppService com os comandos seguintes:

```powershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a>Listar recursos implementados

Pode utilizar o cmdlet `Get-AzureRmResource` para listar os recursos em execução no Azure. O exemplo seguinte mostra os recursos acabados de criar no novo grupo de recursos.

```powershell-interactive
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```Output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westeurope Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westeurope Microsoft.Compute/disks
myLinuxVM                                             westeurope Microsoft.Compute/virtualMachines
myWindowsVM                                           westeurope Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westeurope Microsoft.Compute/virtualMachines/extensions
myNic1                                                westeurope Microsoft.Network/networkInterfaces
myNic2                                                westeurope Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westeurope Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westeurope Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westeurope Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westeurope Microsoft.Network/publicIPAddresses
MYvNET1                                               westeurope Microsoft.Network/virtualNetworks
MYvNET2                                               westeurope Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westeurope Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a>Eliminar recursos

Para limpar a sua conta do Azure, tem de remover os recursos criados neste exemplo. Pode utilizar os cmdlets `Remove-AzureRm*` para eliminar recursos de que já não precisa. Para remover a VM do Windows criada, utilize o seguinte comando:

```powershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

Ser-lhe-á pedido para confirmar se quer remover o recurso.

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

Também pode utilizar o comando para eliminar muitos recursos ao mesmo tempo. Por exemplo, o comando seguinte elimina todos os recursos "MyResourceGroup" do grupo de recursos que utilizámos em todos os exemplos deste tutorial de Introdução. Esta ação remove o grupo de recursos e todos os recursos no mesmo.

```powershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

Esta ação pode demorar vários minutos a concluir.

## <a name="get-samples"></a>Obter exemplos

Para saber mais sobre as formas como pode utilizar o Azure PowerShell, veja os nossos scripts mais comuns para [VMs do Linux](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Vms do Windows](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Aplicações Web](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) e [Bases de Dados SQL](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).

## <a name="next-steps"></a>Passos seguintes

* [Iniciar sessão com o Azure PowerShell](authenticate-azureps.md)
* [Gerir subscrições do Azure com o Azure PowerShell](manage-subscriptions-azureps.md)
* [Criar principais de serviço no Azure com o Azure PowerShell](create-azure-service-principal-azureps.md)
* Leia as Notas de versão sobre a migração de uma versão mais antiga: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).
* Obter ajuda da comunidade:
  * [Fórum do Azure no MSDN](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [Stackoverflow](http://go.microsoft.com/fwlink/?LinkId=320213)
