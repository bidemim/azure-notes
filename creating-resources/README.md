# Creating resources in Azure
A resource in an Azure is a manageable item, think virtual machines, compute resources, network resources etc. No resource is actually stand alone, resources need to be connected in order to function. 

## Ways to create resources
1. The Azure Portal - a graphical interface that supports point and click to create and deploy resources. It is quite easy and would not be covered in my notes.

2. Azure CLI - The command line interface or CLI uses the terminal to manage resources. The CLI can be accessed from the Azure Portal or used locally with the authentication and authorization.

3. Infrastructure as Code (IaC) - IaC let's you create services using a programming interface.  Using this method ensures consistency and supports version control. Which means you can do a rollback easily if needed. Some prominent IaC providers are - Terraform (and its open source fork OpenTofu), Ansible, Pulumi, Chef, Puppet etc. 
Azure also supports Bicep (and ARM templates?) which are specific to Microsoft Azure.    

## Virtual machines (VM). 
To create a VM, other dependent or related items also need to be created. These are:
- The VM
- Disks for storage
- Virtual network
- Network interface to communicate on the network
- Network Security Group (NSG) to secure the network traffic
- An IP address (public, private, or both)

