# FRT Project


# Reading Public Library
#azurelink https://witty-river-0a74cdd10.3.azurestaticapps.net

## Project Statement
Inadequate access to essential study materials and limited awareness of available college library resources hinder students' academic success and effective utilization of educational facilities.

### Industry Type - Ed Tech.

## Project Description
The core idea of my project is to create a comprehensive and accessible reading public library website that serves as a valuable resource for students by providing past year papers, books, and information about library facilities in the college. The project aims to address the problem of limited access to study materials and resources, as well as the need for promoting the college library's services and offerings. It addresses the need for accessible and organized study materials, which can significantly aid students in their academic pursuits. Additionally, it tackles the underutilization of college library facilities by promoting them effectively through the website.

## Azure Services Used

### 1. Static Web Apps
Azure Static Web Apps is a cloud service provided by Microsoft Azure that is used for hosting and deploying static web applications. Static web apps are websites or web applications that consist of HTML, CSS, JavaScript, and other static assets, but do not have server-side logic or dynamic content generation.
Azure Static Web Apps is a versatile platform that is well-suited for hosting a wide range of web applications, including blogs, e-commerce sites, documentation sites, and more, as long as the primary content is static in nature. It simplifies the deployment and management of static web content while offering features for authentication, scalability, and integration with serverless APIs when needed.

1. Hosting Static Websites: Azure Static Web Apps can host static websites and web applications, making it easy to deploy and serve HTML, CSS, JavaScript, images, and other static assets to users globally.

2. Continuous Deployment: It integrates with popular source code repositories like GitHub, GitLab, and Bitbucket, allowing developers to set up automated deployment pipelines. When you push changes to your code repository, Azure Static Web Apps automatically builds and deploys the updated content.

3. Serverless APIs: Azure Static Web Apps can also host serverless APIs using Azure Functions. This means you can combine static content with serverless backend functionality, making it suitable for building complete web applications.

4. Global Content Delivery: Content is distributed through Azure Content Delivery Network (CDN), ensuring low latency and high availability for users around the world.

### 2. Storage Accounts
Azure Storage Accounts are a fundamental and versatile service within Microsoft Azure that provide cloud-based storage solutions for various data types. They serve a wide range of purposes and use cases, making them a crucial component of many Azure applications and services. Here are some of the key purposes and use cases of Azure Storage Accounts:

1. Data Storage: Azure Storage Accounts are primarily used to store various types of data, including:

    1.1 Blob Storage: Used for storing unstructured data like images, videos, documents, backups, and more. It's commonly used for media storage, data archival, and content distribution.

    1.2 File Storage: Offers fully managed file shares in the cloud, suitable for applications that require shared file systems. It's often used for application data and user shares.

    1.3 Queue Storage: Provides messaging between components of cloud applications, enabling communication and coordination between different parts of an application.

2. Data Backup and Recovery: Azure Storage Accounts can be used for data backup and disaster recovery. You can store backups of on-premises or Azure-based data in Storage Accounts for safekeeping.

3. Static Website Hosting: You can use Azure Storage to host static websites, which is a cost-effective way to host simple websites without the need for a web server.
## Prerequisties
1. Azure Portal Subcription
2. Full Stack Development
3. VS Code

## Step-By-Step Implementation

### Creating the Website
Started by developing our frontend website using HTML, CSS, and JavaScript.


HTML is the backbone of a web page. It provides the structure and content of a webpage, defining elements like headings, paragraphs, links, images, forms, and more.


CSS is used for styling and formatting the visual presentation of a web page. It defines how HTML elements should appear, including aspects like layout, colors, fonts, and spacing.


JavaScript is a dynamic scripting language used to add interactivity and behavior to web pages. It enables functionalities such as form validation, animations, real-time updates, and more.


In the end this is the website that is finally done.

<img width="1792" alt="Screenshot 2023-09-15 at 00 20 19" src="https://github.com/Simonithanvi3101/prop/assets/85806856/fc082a57-c44b-46c5-8abb-252fb9da29d1">


### Using Azure Servies Required

If you don't already have an Azure account, sign up for one at https://azure.com. You may need to provide payment information, but Azure offers a free tier with limited resources, Here we will be using our student developers pack.
<img width="1792" alt="Screenshot 2023-09-15 at 00 26 30" src="https://github.com/Simonithanvi3101/prop/assets/85806856/a9774c26-e118-4910-903f-55f13d50b833">

#### Create a Static Web App:
Static Web Apps is a service on Azure designed for hosting static websites with serverless APIs. 


To create a Static Web App:


a. Go to the Azure Portal (https://portal.azure.com/).


b. Click on "Create a resource" and search for "Static Web Apps."


c. Click "Create" and follow the wizard to configure your app.


d. Connect your GitHub repository or other supported source control options to deploy your website automatically.


Configure Deployment:
During the Static Web App creation process, you will need to specify the source code repository, branch, and build settings. Configure these settings to point to your frontend website's source code.
This is the final resource made. 
And we get the web link here i.e. https://witty-river-0a74cdd10.3.azurestaticapps.net

<img width="1094" alt="Screenshot 2023-09-15 at 00 36 09" src="https://github.com/Simonithanvi3101/prop/assets/85806856/e237ed23-f7bf-447c-86d4-92f1a08f45ba">

### Create Storage Accounts And its Containers

#### Set Up a Storage Account:
Azure Storage Accounts are used to store your website's static files (HTML, CSS, JavaScript, images, etc.). To create a Storage Account:


a. In the Azure Portal, click on "Create a resource" and search for "Storage Account."


b. Configure the storage account settings, including the resource group and location.


c. Choose the storage account type (e.g., Standard or Premium).


d. Configure the advanced settings if necessary.


Upload Website Files to Storage Account:
Once your Storage Account is set up, use tools like Azure Storage Explorer or Azure CLI to upload your frontend website files to a container within your Storage Account.

Configure Static Website Hosting in Storage Account:
In your Storage Account settings, configure static website hosting. Specify the index and error documents if required. You'll receive a URL that points to your static website.

Update DNS (Domain Name System):
If you have a custom domain, update your DNS settings to point to the URL provided by your Azure Storage Account's static website hosting. This will allow users to access your website using your custom domain name.

Testing and Monitoring:
Test your website thoroughly to ensure that it's functioning correctly. You can also set up monitoring and analytics using Azure Application Insights or other monitoring tools to track your website's performance.

Scale and Manage:
As your website grows, you can use Azure's scaling options to handle increased traffic. You can also manage your website's resources and configurations through the Azure Portal.

<img width="1094" alt="Screenshot 2023-09-15 at 00 43 55" src="https://github.com/Simonithanvi3101/prop/assets/85806856/609cbec5-dba8-4791-a166-df9e99292ab3">

#### Creating containers
Azure Storage Containers are a way to organize and manage objects within Azure Blob Storage, which is designed for storing unstructured data such as documents, images, videos, and backups. 
1. Navigate to your Azure Storage Account in the Azure Portal.
2. In the left-hand menu, select "Containers."
3. Click the "+ Container" button to create a new container.
4. Provide a unique name for the container. Container names must be lowercase and can include letters, numbers, and hyphens.

This is the Container that we created:
<img width="1094" alt="Screenshot 2023-09-15 at 00 55 04" src="https://github.com/Simonithanvi3101/prop/assets/85806856/5a2d09ff-ab26-4f27-9cf1-42cfb5732f7c">


Further we import all the images, files and folder to the Container so if lost our data from the hardrive we can fetch it back from here.
<img width="1094" alt="Screenshot 2023-09-15 at 00 57 36" src="https://github.com/Simonithanvi3101/prop/assets/85806856/9cad7a91-5274-47ce-b9f0-ddccec9dc9b7">
<img width="1094" alt="Screenshot 2023-09-15 at 00 57 56" src="https://github.com/Simonithanvi3101/prop/assets/85806856/89e73d71-330b-42f0-bc98-ed11464994e3">



## Video Link
https://drive.google.com/file/d/1Z13mE1jmD22cHEGJ5nl1pSHtsttiy_7u/view?usp=sharing
