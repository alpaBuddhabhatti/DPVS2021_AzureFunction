# Introduction 

**Azure function**
Resize Image as soon as **Picture 2.jpg** added to **input** container due to **Blob trigger** , Azure function execute code and resize same image with two new diffrent size and store images to **output** container.
Following Azure resources have been used .
Azure Storage Account
Azure Key Valut
Azure Function App
Azure Function

There are two code repositoy 
1. **AZDEV-DSP_FA** - Azure Function code (code repo)   
2. **Deployment** - Azure function deployemnt (ARM tempalte project)

# Getting Started

1. Clone repository to your local machine using VScode or Visual studio 2017/2019

2. Create storage Account in Azure portal to execute Azure funtion in locally

3. Copy connection string of Storage Account 

4. Open AZDEV-DSP_FA/local.settings.json file and past it in place of "YOUR CONNECTIONSTRING"

5. Portal.azure.com => your storage account => Create New Container as "**input**"=> Upload any Image file(Rename as **Picture 2.jpg** and then uplod)

6. Create new contianer as **output** 

7. Now you can run azure funtion apps

8. Portal.azure.com =>upload Same Image file again , you can see azure function will trigger and it will generate two diffrents size file and place to output container

9. Once you happy with execution , you can create CI pipeline using YAML file in Deployemnt repo

10. Then you can create Release pipeline to deploye into TST/SIT/PRD


