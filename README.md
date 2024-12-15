### AzureMLOps-Classifier

Deploying of Classification model using Azure devops, docker and Azure services

## Steps to Deploy the Classification Model

### 1. Clone the Azure Repository
- Create a new project after logging into your Azure account.
- Alternatively, you can clone the Azure repository through **VS Code**:
  1. Click on **Clone in VS Code** in the Azure portal.
  2. Make changes to the files as required.
  3. Push all the updated files back to the repository through VS Code.

### 2. Define a Dockerfile
- Create a `Dockerfile` for your project that specifies:
  - Required dependencies
  - Environment setup
  - Configurations

### 3. Create an Azure Resource Group
- Create an Azure Resource Group using the Azure portal:
  1. Go to the **Resource Groups** section.
  2. Click on **Create**.
  3. Provide a proper name for your resource group.
  4. Click **Review + Create** to finalize.

### 4. Create an Azure Container Registry
- Add an Azure Container Registry (ACR) to host your Docker image:
  1. Navigate to the **Resource Group** you created earlier.
  2. Click on **Add** and search for **Azure Container Registry**.
  3. Provide the necessary details and add it to your resource group.

### 5. Define an Azure Pipeline
- Set up an Azure DevOps pipeline to build and deploy the Docker image:
  1. Log in to your **Azure DevOps** account and navigate to your project.
  2. Click on **Pipelines** and create a new pipeline.
  3. Select your repository and configure the pipeline with **Docker**.
  4. Save and run the generated `YAML` file.

### 6. Customize the YAML File
- Modify the `YAML` file to include any additional steps or configurations specific to your project.

### 7. Deploy the Docker Image to Azure Web App
- Use the Azure Container Registry to deploy your Docker image:
  1. Go to the **Azure Container Registry** you created.
  2. Add a **Web App** resource to your resource group.
  3. Name the Web App appropriately and configure it to pull the image from the registry.
  4. Review and create the Web App to complete the deployment.

## Conclusion
Follow these steps to deploy your classification model seamlessly using Azure DevOps and Azure services.