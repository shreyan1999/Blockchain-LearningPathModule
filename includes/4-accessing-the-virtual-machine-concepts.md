# Accessing the Virtual Machine

In this unit, you will distinguish between different ways to connect to your virtual machine that you’ve just deployed in the previous unit.

## Recap of what you just deployed

Once you have deployed Quorum Dev QuickStart, a few resources are deployed in the resource group.

![Screenshot of all the resources created](/media/4.1-Resouces_deployed.png)
The resources deployed on the overview page under Quorum Dev QuickStart are mentioned below:

----------------------------------------------------------------------------------------------------
| Name | Type | Location |
| :---: | :---: | :---: |
| Quorumjx2 | Virtual Machine | West Europe |
| Quorumjx2-nic | Network Interface | West Europe |
| Quorumjx2-nsg | Network Security group | West Europe |
| Quorumjx2-pip | Public IP address | West Europe |
| Quorumjx2-vnet | Virtual network | West Europe |
| Quorumjx2_OsDisk_[……] | Disk | West Europe |

## Options to connect with the Virtual Machine

There are three ways to connect to a virtual machine that’s of interest:

- **SSH**, SSH stands for secure shell and SSH and is an encrypted connection protocol that allows secure sign-ins over unsecured connections.
- **RDP**, stands for remote desktop protocol which provides a user with a graphical interface to connect to another computer over a network connection.
- **Bastion**, is a service you deploy that lets you connect to a virtual machine using your browser and the Azure portal

## Connecting with SSH

With a secure shell (SSH) key pair, you can create virtual machines (VMs) in Azure that use SSH keys for authentication. SSH is an encrypted connection protocol that allows secure sign-ins over unsecured connections. SSH is the default connection protocol for Linux VMs hosted in Azure.  

> [!NOTE]  
>
> Although SSH itself provides an encrypted connection, using passwords with SSH still leaves the VM vulnerable to brute-force attacks.  

> [!TIP]
>
> The recommendation is to connect to a VM over SSH using a public-private key pair, also known as SSH keys.  

The public-private key pair is like the lock on your front door. The lock is exposed to the public, anyone with the right key can open the door. The key is private, and only given to people you trust because it can be used to unlock the door.

## Connecting with RDP

Remote Desktop Protocol (RDP) is a proprietary protocol developed by Microsoft which provides a user with a graphical interface to connect to another computer over a network connection.  

When new to Linux, or for quick troubleshooting scenarios, the use of remote desktop may be easier.

Linux virtual machines (VMs) in Azure are usually managed from the command line using a secure shell (SSH) connection.  

> [!NOTE]
>
> This article details how to install and configure a desktop environment (xfce) and remote desktop (xrdp) for your Linux VM running Ubuntu. To know more visit <https://docs.microsoft.com/en-us/azure/virtual-machines/linux/use-remote-desktop>

## Connecting with Bastion

Azure Bastion is a service you deploy that lets you connect to a virtual machine using your browser and the Azure portal. The Azure Bastion service is a fully platform-managed PaaS service that you provision inside your virtual network. It provides secure and seamless RDP/SSH connectivity to your virtual machines directly from the Azure portal over TLS.  

When you connect via Azure Bastion, your virtual machines do not need a public IP address, agent, or special client software. Bastion provides secure RDP and SSH connectivity to all of the VMs in the virtual network in which it is provisioned.  

Using Azure Bastion protects your virtual machines from exposing RDP/SSH ports to the outside world, while still providing secure access using RDP/SSH. To know more visit [MS Docs](https://docs.microsoft.com/en-us/azure/bastion/bastion-overview)