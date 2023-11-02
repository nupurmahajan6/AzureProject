# Deployment of JobEntry Website using IIS, Load balancer, recovery vault and Multi-factor Authentication.

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



