# Deployment of JobEntry Website using IIS, Load balancer, recovery vault and Multi-factor Authentication.

 Procedure
Step1: Establish a Virtual Network (V-Net) that contains a subnet, and within that subnet(webserver), place a Virtual Machine (VM)

Step2: Now create a two Virtual machine name VM1 and VM2
in one subnet

Step3: Now connect VM1 and VM2 after connecting VM add feature web server(IIS) install the IIS future

Step4: Now deploy web site in VM1 And VM2

Step5: Go to azure portal and check web site working or not, copy the VM1 IP and paste portal.

Step6: Now a create load balancer and add VM’s in load balancer
Load balancer: Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers or resources. It is distributed equally internet traffic toward the available healthy server.

Step 7: Now create recovery vault and add VM1 and VM2 for backup vm’s purpose.
A Recovery Services vault is a storage entity in Azure that houses data. The data is typically copies of data, or configuration information for virtual machines (VMs), workloads, servers, or workstations. You can use Recovery Services vaults to hold backup data for various Azure services such as IaaS VMs (Linux or Windows) and SQL Server in Azure VMs.
Step 8: Now we have use multi-factor Authentication which is second level of security.

Azure Services Used:
1.	Azure VM
2.	Load balancer
3.	Recovery vault
4.	Multi-factor Authentication.

1.Azure VM:
Azure virtual machines are one of several types of on-demand, scalable computing resources that Azure offers. Typically, you choose a virtual machine when you need more control over the computing environment than the other choices offer. This article gives you information about what you should consider before you create a virtual machine, how you create it, and how you manage it. An Azure virtual machine gives you the flexibility of virtualization without having to buy and maintain the physical hardware that runs it. However, you still need to maintain the virtual machine by performing tasks, such as configuring patching, and installing the software that runs on it.
Applies to: ✔️ Linux VMs ✔️ Windows VMs ✔️ Flexible scale sets

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/eb5f1e5f-db77-468e-91ee-d9853018269e)

IIS Service:
IIS stands for Internet Information Services  is a flexible, general-purpose web server from Microsoft that runs on Windows systems to serve requested HTML pages or files.
An IIS web server accepts requests from remote client computers and returns the appropriate response. This basic functionality allows web servers to share and deliver information across local area networks (LAN), such as corporate intranets, and wide area networks (WAN), such as the Internet.
A web server can deliver information to users in several forms, such as static webpages coded in HTML; through file exchanges as downloads and uploads; and text documents, image files and more.

2. Load balancer:
Load balancing refers to efficiently distributing incoming network traffic across a group of backend servers or resources. It is distributed equally internet traffic toward the available healthy server.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/17aa6fb1-77b2-4d10-afba-f5b54f392758)

Azure Load Balancer operates at layer 4 of the Open Systems Interconnection (OSI) model. It's the single point of contact for clients. Load balancer distributes inbound flows that arrive at the load balancer's front end to backend pool instances. These flows are according to configured load-balancing rules and health probes. 
A public load balancer can provide outbound connections for virtual machines (VMs) inside your virtual network. These connections are accomplished by translating their private IP addresses to public IP addresses. Public Load Balancers are used to load balance internet traffic to your VMs.
An internal (or private) load balancer is used where private IPs are needed at the frontend only. Internal load balancers are used to load balance traffic inside a virtual network. A load balancer frontend can be accessed from an on-premises network in a hybrid scenario.

3.Recovery vault
A Recovery Services vault is a storage entity in Azure that houses data. The data is typically copies of data, or configuration information for virtual machines (VMs), workloads, servers, or workstations. You can use Recovery Services vaults to hold backup data for various Azure services such as IaaS VMs (Linux or Windows) and SQL Server in Azure VMs. Recovery Services vaults support System Centre DPM, Windows Server, Azure Backup Server, and
more. Recovery Services vaults make it easy to organize your backup data, while minimizing management overhead.
Recovery Services vaults are based on the Azure Resource Manager model of Azure, which provides features such as:
•	Enhanced capabilities to help secure backup data: With Recovery Services vaults, Azure Backup provides security capabilities to protect cloud backups. The security features ensure you can secure your backups, and safely recover data, even if production and backup servers are compromised.
•	Central monitoring for your hybrid IT environment: With Recovery Services vaults, you can monitor not only your Azure IaaS VMs but also your on-premises assets from a central portal.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/71f86ab2-9757-4a87-a935-c5a87cae0efb)

•	Azure role-based access control (Azure RBAC): Azure RBAC provides fine-grained access management control in Azure. Azure provides various built-in roles, and Azure Backup has three built-in roles to manage recovery points. Recovery Services vaults are compatible with Azure RBAC, which restricts backup and restore access to the defined set of user roles.
•	Soft Delete: With soft delete, even if a malicious actor deletes a backup (or backup data is accidentally deleted), the backup data is retained for 14 additional days, allowing the recovery of that backup item with no data loss. The additional 14 days of retention for backup data in the "soft delete" state don't incur any cost to you.
•	Cross Region Restore: Cross Region Restore (CRR) allows you to restore Azure VMs in a secondary region, which is an Azure paired region. By enabling this feature at the vault level, you can restore the replicated data in the secondary region any time, when you choose. This enables you to restore the secondary region data for audit- compliance, and during outage scenarios, without waiting for Azure to declare a disaster (unlike the GRS settings of the vault).

4.Multi-factor Authentication (MFA):
MFA is a second level of security to the users.
From Active Directory we can assign the authentication to user.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/3039ed2f-02cb-4f2c-b0d2-6b8f7e3031c8)

Suppose there is admin and multiple users.
If any user forget the pasword then he/she will go to admin and then can reset the password.
But if many users forget the password then all user have to go to admin which will increase burden on the admin.
So to tackle this problem self service password reset is the solution
By self service password reset the user can reset the password without ging to admin.



IMPLEMENTATION

Create Virtual Machine (VM1).

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/b5c482eb-4609-4c2c-86d3-d2f8ec9cd0c9)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/ec4c1535-f19c-49a9-abde-907e2b0dce6b)

Now connect the VM1 by RDP.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/40aa9432-60f9-4078-a586-5af2db466c5e)

Now add feature web server(IIS)deploy the Web site in VM1 

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/39eab06c-9fb8-4ebe-b65d-7349087f417c)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/c1f50fd3-46d5-46f3-a523-4228fb4ed9f8)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/7b3c2d39-230d-4c79-96ee-d2f0d19d1e8a)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/d43ad09c-fca3-4acc-92d8-c4e0bdd9ffa2)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/f182e962-8e70-4df7-8c10-a417ae3571bc)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/588c5c70-0411-4ba9-857a-36b6fe08e083)

Now by using the IP we can access the website .

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8d64b601-1aeb-41ae-8451-714e649b4884)

Now by using the Domainname we can access the website .

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/255f4d72-92ea-4b03-b094-bd959ced3aa5)

Create Second Virtual Mahine (VM2).

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8e8b278c-7fc4-4e4b-bfca-695ddc746542)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/83625aff-3e49-4bda-b557-d2e2c82e6dea)

Now connect the VM2 by RDP.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8ae2ecd0-797c-4020-b670-7d8936823973)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/ef08d224-1833-493c-ab69-537e4f2254a1)

Now add feature web server(IIS)deploy the Web site in VM2

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/39eab06c-9fb8-4ebe-b65d-7349087f417c)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/c1f50fd3-46d5-46f3-a523-4228fb4ed9f8)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/7b3c2d39-230d-4c79-96ee-d2f0d19d1e8a)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/d43ad09c-fca3-4acc-92d8-c4e0bdd9ffa2)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/f182e962-8e70-4df7-8c10-a417ae3571bc)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/588c5c70-0411-4ba9-857a-36b6fe08e083)

Now by using the IP we can access the website .

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/2e5ade31-03ce-42d9-8682-225a31fc6631)

Now by using the Domainname we can access the website .

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/5418bad8-6a49-4095-aa06-d31e12e26e74)






Now Create Load Balancer.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/ffbce7a2-1f83-40d1-8e9a-fada2fa742d1)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/a91dd379-e724-47f7-bdbd-dc529aa8c5dc)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/e35d3f59-53e9-4366-8947-1696ec735a8f)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/b5e3b10d-3506-4d33-903a-7daeb992dec1)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/fbb22724-b93b-4381-9536-fa4fca0b36e7)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/0d4dcc22-ff5a-4dd3-bde3-57e6129fe5bf)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8188d976-7ecc-4084-954a-bbf5767de0d4)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/754f7d3c-e321-4a94-aaa6-6e1de38b914c)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/b12dd439-b53a-43eb-87f4-64701e57436d)

Now Copying th IP address of Load Balancer we can see the webite sometimes we can see the website of VM1 and sometime of VM2 .

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/2561924d-7d2d-4c72-ac36-2d214775e7ed)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/b59b69a7-3ede-4edd-bddd-c8d47a5699dc)

Create a recovery vault for Virtual machine (VM1) backup purpose

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/578d26c5-4021-4e56-9036-e863def6d480)

Select virtual machine backup option and after that click on add button and add two Virtual machine

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/20bf6518-cdea-4bcd-aba9-a1ed17fd53a4)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/7fb5b630-a277-4cd9-b925-e27530373e7f)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/23cad358-5278-4d1b-b788-3d04f58dfb38)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/c25d5eab-adf6-4507-9088-eb598f64c230)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/10f8b030-f436-421c-88c5-1edfb6f988e2)

Then we backed up both the VMs using Azure Recovery Service Vault.

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/36bdce74-8471-4d3b-9ee6-f4f000ee5429)

Multi Factor Authentication (MFA).
Active Directory >> New User > Create

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8e0e1e68-db80-47a7-af90-d7c357153cbe)

Assign a role (Global Administrator)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/bcde0716-9f70-464a-a464-006153ab2c2e)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/749f798d-8316-4c36-8807-c5423d1c249e)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/fe03ffda-5840-4c57-8628-3c3a386cfde0)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/9c24c4d7-86fc-4d3d-b4ec-2a399395b72e)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/3000ff16-c6d6-4280-ae43-a40c2820339a)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/ae49ea4d-fb22-43fc-9db7-2d42cb57672c)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/58cddbf7-0e13-49ac-b620-6eed74fc5ad2)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/0d3467bd-fb45-47f7-be93-df524a0e2eb6)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/9c03e5db-ce6d-4fab-9ba7-d66c058c76b5)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/c5b85451-55aa-4de2-9abd-b897cc75b4d9)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/8b0a3aed-b720-45ac-b2db-edf6f63c96df)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/405e7089-d57c-41cb-9f0f-2add0e5fdd4e)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/4747c7db-ba0e-4969-be99-387eae42f78d)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/937250da-3af6-45c5-afa2-2f037b7f7525)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/e2c786df-ee05-4725-8748-6e8fe20f1710)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/195807a4-a3e3-4972-b01f-f1cc6d9d3a8d)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/93b5d93e-fd77-48bc-98a1-fd68fefff32b)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/7615fa08-272f-4dd4-bd95-edf8d06b03e0)

![image](https://github.com/nupurmahajan6/AzureProject/assets/147131064/eee73004-3326-47fc-901a-dbd098a6ba4b)



