# Azure Resume Website
This is my solution to the Azure Resume Challenge.<br/>
You can view the live version [here](https://www.jacobdornbusch.com).

## Architecture Diagram
![Diagram](https://i.imgur.com/BbestzP.png)
## Project Overview

This project combines front-end and back-end resources to create a friendly and readable website for the Azure Resume Challenge. The website includes a visitor counter feature that fetches data from an Azure Function through an API call.

## Azure Technologies Used

The following Azure technologies were utilized in this project:

- Azure CosmosDB
- Azure Functions
- Azure Storage
- Azure CDN

## Prerequisites

Before getting started, make sure you have the following prerequisites:

- GitHub account
- Azure account
- Azure CLI
- .NET Core 6.0 LTS
- Azure Functions Core Tools
- Visual Studio Code
- Visual Code Extensions:
  - Azure Functions Extensions
  - C# Extension
  - Azure Storage Extension

## Frontend

The front-end of this project is a static website built with HTML, CSS, and JavaScript. It utilizes a visitor counter feature that retrieves data from an Azure Function through an API call. 

## Backend

The back-end of this project consists of an HTTP triggered Azure Function with Cosmos DB input and output binding. The Function is responsible for retrieving a Cosmos DB item, incrementing its value by 1, saving it, and returning the updated value to the caller. 

## Testing

Testing is an important part of the development process. While the tests in this project are simple, they were still implemented. The resources used for testing are specific to .NET, but the concepts can be applied to any programming language.

## CI/CD

Continuous Integration and Continuous Deployment (CI/CD) are crucial for efficient development workflows. In this project, GitHub Actions were utilized to deploy the static site to blob storage and deploy the Azure Function to Azure.

## Project Setup

To set up this project, follow these steps:

1. Open the "frontend" folder, which contains the website files.
2. In the "main.js" file, you'll find the code for the visitor counter.
3. Open the "backend" folder, which contains the API files.
4. Create an Azure Resource Group through the Azure portal.
5. Create an Azure Cosmos DB account through the Azure portal.
6. Create an Azure Function locally using the Azure CLI.
7. Deploy the local Azure Function to Azure for production using the Azure Functions extension in Visual Studio Code.
8. Deploy the "frontend" folder to Azure Blob Storage using the Azure Storage extension in Visual Studio Code.
9. Update the CORS settings on the Azure Function to allow calls from the Azure Blob Storage URL.
10. Create an Azure CDN for the Azure Blob Storage.
11. Add a custom domain to the CDN.
12. Enable HTTPS on the Azure CDN.
13. Add the custom domain to the CORS policy for the Azure Function.
