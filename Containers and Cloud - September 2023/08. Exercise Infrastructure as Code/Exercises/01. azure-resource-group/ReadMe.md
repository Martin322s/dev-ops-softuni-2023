# Creating an Azure Resource Group with Terraform

In this guide, we will walk you through the process of creating an Azure Resource Group using Terraform. Azure Resource Groups are logical containers for managing and organizing Azure resources. We will go through the steps to set up your Terraform configuration and deploy an Azure Resource Group.

## Prerequisites

Before we begin, ensure you have the following prerequisites in place:

1. Azure CLI installed on your local machine.
2. Terraform installed on your local machine.
3. An Azure account with the necessary permissions.

## Step 1: Initialize your Terraform configuration

Open a terminal (e.g., PowerShell) and create a new folder for your Terraform configuration. You can name it as per your choice. Navigate to this folder in your terminal.

mkdir terraform-azure-rg
cd terraform-azure-rg` 

## Step 2: Authentication with Azure CLI

Before you can create Azure resources with Terraform, you need to authenticate using the Azure CLI. Run the following command to log in to your Azure account:

`az login` 

Follow the authentication process in your web browser if prompted.

## Step 3: Create your Terraform configuration file

Now, create a Terraform configuration file (e.g., `main.tf`) in your folder and open it using a text editor.

`touch main.tf` 

Add the following code to your `main.tf` file:

`provider "azurerm" {
  features {}
}

resource "azurerm_resource_group" "example" {
  name     = "your-resource-group-name"
  location = "East US" # Replace with your desired Azure region
}` 

In this code:

-   We define the Azure provider block, and within it, we specify the features required.
-   We create an Azure Resource Group using the `azurerm_resource_group` resource. Make sure to replace `"your-resource-group-name"` with your preferred name and set the appropriate `location`.

-   ## Step 4: Initialize, Format, Validate, and Apply your Terraform configuration

Now, let's initialize your Terraform configuration, format it, validate it, and apply it to create the Azure Resource Group.

1.  Initialize the configuration:

`terraform init` 

2.  Format the configuration to ensure consistent style:

`terraform fmt` 

3.  Validate the configuration to check for any errors:

`terraform validate` 

4.  Apply the configuration to create the Azure Resource Group:

`terraform apply` 

You will be prompted to confirm the creation. Type "yes" and press Enter to proceed.

## Step 5: Verify in Azure Portal

After Terraform has successfully created the Azure Resource Group, you can verify its existence by logging into the [Azure Portal](https://portal.azure.com/) in your web browser.

## Step 6: Deleting the Resource Group

If needed, you can also use Terraform to delete the Azure Resource Group you created. Run the following command:

`terraform destroy` 

Again, you will be prompted to confirm the deletion. Type "yes" and press Enter.
