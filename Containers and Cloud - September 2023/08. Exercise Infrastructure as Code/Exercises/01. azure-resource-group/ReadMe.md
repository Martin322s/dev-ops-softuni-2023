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
