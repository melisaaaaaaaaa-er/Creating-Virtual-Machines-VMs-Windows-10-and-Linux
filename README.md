# Creating Virtual Machines (VMs) - Windows 10 and Linux

<h2>Deployment and Configuration Steps:</h2>

<h3>Windows 10</h3>

![1](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/eaddde80-7823-4cad-9bd0-d1c8ec7ee0de)

To get started, select the “Virtual Machines” service option.

There are multiple ways to find and access a service on Azure. The easiest way is to use the search bar at the top of the home page if a service does not immediately show up on the main interface.

#
![2](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/1691e583-d44e-4f81-946f-51a705da50cf)

Once in the virtual machines interface, select “+ Create → Azure virtual machine”.

#
![3](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/d2df37fb-aba6-43ba-899b-3741534cca28)

Select the subscription and resource group you want to host the VM in.

The two VMs created for the project should be in the same resource group.

Give the VM a name, and select the ISO image to be used for the VM. This VM will be a Windows 10 machine, so I selected the “Windows 10 Pro” ISO image.

#
![4](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/c61a1e23-48a9-478f-b119-d0295486e29f)

Select the hardware resources size for the VM. Higher resource use has higher costs associated with it, so be sure to select a size based on both the needs of the VM as well as budget constraints.

Input the Administrator account credentials (username + password).

#
![5](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/b27267c1-46b8-476d-a12e-776128920a6f)

Check off the licensing terms-and-conditions box.

#
![6](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/b8feedf3-bbf5-4360-a95c-bd28376c7f17)

In the “Networking” configuration panel, select the “Create new” option under “Virtual network”.

Give the new virtual network card a name and select “OK” at the bottom.

This virtual network card will be used by both the Windows 10 and Ubuntu linux VMs as they need to be on the same network for the network testing portion of the project.

#
![7](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/44b63dfe-e466-4ec7-8fdd-2d9113cf3187)

Select “Review + create”.

#
![8](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/bd659978-fffc-47b9-b505-9ab1fd99bbc9)

Once the VM has been validated, select “Create”.

#
![9](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/d9056f76-40b8-416d-b5e8-ef1a93303255)

The Windows 10 VM deployment in progress.

#
<h3>Ubuntu Linux VM</h3>

![10](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/8b95a6e9-baab-4603-9f7f-f9a084e47b50)

Go back to the “Virtual machines” service interface.

Select “+ Create → Azure virtual machine”. 

#
![11](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/32deafd8-9032-483f-964b-412cd7539a96)

Select the subscription and resource group you want to host the VM in.

The two VMs created for the project should be in the same resource group.

Give the VM a name, and select the ISO image to be used for the VM. This will be an Ubuntu linux machine so I selected the Ubuntu Server 20.04 LTS ISO image.

#
![12](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/3b726bb7-c0fd-497f-aa2e-bced57dc5168)

Select the hardware resources size for the VM. The same factors apply here as in the previous VM creation process.

Select “Password” for the authentication type and input the Administrator account credentials (username + password).

#
![13](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/123dfc7f-6e02-4003-a27d-12944697624b)

In the “Networking” configuration interface, select the virtual network card created previously, then “Review + create”.

NOTE: VMs can be in different resource groups and still preserve network connectivity with each other as long as they share the same virtual network card. For the sake of simplicity, the VMs in this project are placed in the same resource group.

#
![14](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/295d4596-bd32-42ec-b0e3-79d242d0351c)

Once the VM is validated, select “Create”.

#
![15](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/f1871fe1-6be4-46e3-81a6-896bb9cd8c8e)

Here are the two VMs.

#
![15 5](https://github.com/melisa-er/Creating-Virtual-Machines-VMs-Windows-10-and-Linux/assets/157723219/d0729fdd-f88f-4789-9853-ab5e9745cb41)

The resources for each VM can be seen in the resource group they use.
