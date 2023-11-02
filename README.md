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


Now by using the Domainname we can access the website .



(ADD new SS of Website images change kiya he vo wala)



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





Now by using the Domainname we can access the website .
(ADD new SS of Website images change kiya he vo wala)






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








