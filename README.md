# Deploy Node JS Application with Mongo DB

Azure App Service is a platform as a service that provides a platfrom to easily deploy applications of different stack.
In this task I deployed a Node JS application to Azure App Service and created a Cosmo DB Server for the database credentials. Below are the steps I took
- Create a Resource Group in US East to add resources 
![resource-group](./images/app-service-rg.png)

- Create An Azure Cosmos DB and note the credentaials for authenticaiton which are the Cosmos Account Name, Cosmos Primary password and Connection URL
![MongoDb](./images/cosmos-db.png)
-  Create a Web APP in the resource group and skip the Database Fields. 
![AppService](./images/app-service.png)

- Created a virtaul Network and Subnet in the Resource Group during the creation of the Web App Service

- Enabled Continous Deployment and Linked my github account to App service 

- I choose the Basic Service Plan (B1)
![serviceplan](./images/appservice-plan.png)

- The deployed link is https://contour-air.azurewebsites.net/

![deployed Url](./images/deployed-url.png)

- Upgraded App Service plan to Premium V3 P0V3 to enable staging slot feature
![app-service-2](./images/app-service-plan-12.png)

- Added the Staging Slot
![deployed Url](./images/staging-slot.png)

- The deployed staging slot link is https://contour-air-staging.azurewebsites.net/