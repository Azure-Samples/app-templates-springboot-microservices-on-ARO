# Spring Boot PetClinic Microservices Application Deployed to Azure Red Hat Openshift (ARO)
> [!NOTE]
> For Spring Boot applications, we recommend using Azure Spring Apps. See [Java Workload Destination Guide](https://aka.ms/javadestinations) for advice. 

## Description 
In this sample app template, the PetClinic application (a Spring Boot based app) is containerized and deployed to an Azure RedHat Openshift (ARO) cluster secured by Azure Firewall

## Deploy Spring Boot apps using Azure Red Hat Openshift (ARO) and Azure Services:

--
Tech stack:

- Azure Container Registry (ACR)
- MySql DB
- Azure Red Hat Openshift (ARO) Cluster
- Azure Infra (Hub & Spoke Topology)
- Azure Infra (VNet Peering)
- Azure Fire Wall
- Azure Bastion
- Github Actions
- Bicep
- Docker
- Maven
- Springboot

---

## Introduction

This is a quickstart template. It deploys the following:

* Deploying PetClinic App:
  * Provisioning Azure Infra Services with BICEP
  * Create the spring-petclinic- build with Maven
  * Create an Azure Container Registry
  * Push your app to the container registry
  * Create an Azure Redhat Openshift (ARO) Cluster
  * Deploy the image to your ARO cluster
  * Verify your container image

* PetClinic on Automated CI/CD with GitHub Action  
  * CI/CD on GitHub Action
  * CI/CD in action with the app

> Refer to the [App Templates](https://github.com/microsoft/App-Templates) repo Readme for more samples that are compatible with [AzureAccelerators](https://github.com/Azure/azure-dev/).

## Prerequisites
- Local shell with Azure CLI installed or [Azure Cloud Shell](https://ms.portal.azure.com/#cloudshell/)
- Azure Subscription, on which you are able to create resources and assign permissions
  - View your subscription using ```az account show``` 
  -  If you don't have an account, you can [create one for free](https://azure.microsoft.com/free).  

## Getting Started
### Fork the repository

1.  Fork the repository by clicking the 'Fork' button on the top right of the page.
This creates a local copy of the repository for you to work in. 

2.  Configure GITHUB Actions:  Follow the insturctions in the [GITHUB_ACTIONS_CONFIG.md file](https://github.com/Azure-Samples/app-templates-springboot-app-on-ARO/blob/main/.github/GITHUB_ACTIONS_CONFIG.md) (Located in the .github folder.)

3.  Run the workflow 
   * If workflows are enabled for this repository it should run automatically. To enable the workflow run automatically, Go to Actions and enable the workflow if needed.
   * Workflow can be manually run 
     + Under your repository name, click Actions .
     + In the left sidebar, click the workflow "Build and Deploy Application".
     + Above the list of workflow runs, select Run workflow .
     + Use the Branch dropdown to select the workflow's main branch, Click Run workflow .
  

# Pet Clinic Website

<img width="1042" alt="petclinic-screenshot" src="https://cloud.githubusercontent.com/assets/838318/19727082/2aee6d6c-9b8e-11e6-81fe-e889a5ddfded.png">


Congratulations! Now you have your containerized Java Sping Boot App deployed on AKS with supported JDK pushed to your ACR. 

# Pet Clinic Website - IP Address 

4. If you wish to view the PetClinic deployment, follow the steps listed below:
- Log into the Azure Portal
- Nagivate the the "petstore_spoke_eastus" Resource Group


