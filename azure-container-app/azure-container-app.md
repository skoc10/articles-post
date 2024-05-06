![](./images/azure-container-abp.png)

# AZURE CONTAINER APPS DEPLOYMENT WITH ABP

In this article, we explore the seamless deployment of an ABP Framework MVC project to Azure Container Apps. Azure Container Apps is a fully managed Azure service that allows you to deploy and run containerized applications without having to manage the underlying infrastructure. It provides a simple and cost-effective way to deploy and scale your applications.

To get started, you will need an ABP Framework MVC project that you want to deploy. If you don't have one, you can [create a new project using the ABP CLI](https://docs.abp.io/en/abp/latest/Startup-Templates/Application). You will also need [an Azure subscription](https://azure.microsoft.com) and [an Azure SQL database](https://azure.microsoft.com/en-gb/products/azure-sql).

Before creating Azure container apps resources and deploying the ABP Framework MVC project, I show you how you can effortlessly create Docker images and push them to Docker Hub, leveraging the pre-configured Docker file and scripts that come with the ABP MVC framework.

To create a Docker image for your ABP Framework MVC project, navigate to `etc/build/build-images-locally.ps1` and fix the script to match your Docker Hub username and image name. Then, run the script to build the Docker image locally.

![Build Docker Image](./images/build-docker-image.png)

Next, check the Docker Hub repository to confirm that the image has been pushed successfully.

![Docker Hub Repository](./images/docker-hub-repository.png)