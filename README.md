# Creating Virtual Machines (VMs) - Windows 10 and Linux

<h3>Purpose</h3>

- creating virtual machines (VMs) on Microsoft Azure - Windows and Linux.

<h2>Deployment and Configuration Steps:</h2>

<h3>Windows 10</h3>

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/1.png"/>

To get started, select the “Virtual Machines” service option.

There are multiple ways to find and access a service on Azure. The easiest way is to use the search bar at the top of the home page if a service does not immediately show up on the main interface.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/2.png"/>

Once in the virtual machines interface, select “+ Create → Azure virtual machine”.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/3.png"/>

Select the subscription and resource group you want to host the VM in.

The two VMs created for the project should be in the same resource group.

Give the VM a name, and select the ISO image to be used for the VM. This VM will be a Windows 10 machine, so I selected the “Windows 10 Pro” ISO image.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/4.png"/>

Select the hardware resources size for the VM. Higher resource use has higher costs associated with it, so be sure to select a size based on both the needs of the VM as well as budget constraints.

Input the Administrator account credentials (username + password).

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/5.png"/>

Check off the licensing terms-and-conditions box.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/6.png"/>

In the “Networking” configuration panel, select the “Create new” option under “Virtual network”.

Give the new virtual network card a name and select “OK” at the bottom.

This virtual network card will be used by both the Windows 10 and Ubuntu linux VMs as they need to be on the same network for the network testing portion of the project.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/7.png"/>

Select “Review + create”.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/8.png"/>

Once the VM has been validated, select “Create”.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/9.png"/>

The Windows 10 VM deployment in progress.

#
<h3>Ubuntu Linux VM</h3>

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/10.png"/>

Go back to the “Virtual machines” service interface.

Select “+ Create → Azure virtual machine”. 

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/11.png"/>

Select the subscription and resource group you want to host the VM in.

The two VMs created for the project should be in the same resource group.

Give the VM a name, and select the ISO image to be used for the VM. This will be an Ubuntu linux machine so I selected the Ubuntu Server 20.04 LTS ISO image.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/12.png"/>

Select the hardware resources size for the VM. The same factors apply here as in the previous VM creation process.

Select “Password” for the authentication type and input the Administrator account credentials (username + password).

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/13.png"/>

In the “Networking” configuration interface, select the virtual network card created previously, then “Review + create”.

NOTE: VMs can be in different resource groups and still preserve network connectivity with each other as long as they share the same virtual network card. For the sake of simplicity, the VMs in this project are placed in the same resource group.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/14.png"/>

Once the VM is validated, select “Create”.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/15.png"/>

Here are the two VMs.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vms-network-activities-images/main/15.5.png"/>

The resources for each VM can be seen in the resource group they use.
