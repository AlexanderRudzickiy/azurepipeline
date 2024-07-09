Overview:

This project demonstrates the use of a self-hosted Azure DevOps agent on a DevOps VM within an Azure environment. The goal is to create a CI/CD pipeline that builds and deploys a basic "Hello, World!" Flask application to a private Azure Kubernetes Service (AKS) cluster using a private Azure Container Registry (ACR).

CI/CD Part:

For the CI/CD part, I have used an Azure DevOps pipeline runned by self-hosted agent on the DevOps VM.

Key Steps:

1. Using VM deployed with terraform.
For future projects, it is recommended to use a pre-built image of Windows Server/Linux that includes common services such as Docker, Azure CLI, kubectl, and more.
3. Setting up VM as Azure DevOps Self-Hosted Agent: The VM is configured to run as a self-hosted agent in Azure DevOps and shown in the agent pool.
4. Azure DevOps integration and service connection configuration: Ensured that our Azure DevOps pipelines utilize self-hosted agent to run CI/CD tasks and have permission to AKS/ACR.
5. Private Deployment: Facilitated the deployment of applications to a private AKS using images stored in a private ACR.

Python code source: https://github.com/Azure-Samples/python-docs-hello-world

Terraform: https://github.com/AlexanderRudzickiy/Private_AKS_with_ACR/tree/main
