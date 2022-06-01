# Web-API-Dock-Image-ACR-Github-Actions

Create necessary resources in the Azure
```
#Optional - This command is only necessary if you're using a local terminal
az login

# Resource Group
ACR_RG_NAME=<RESOURCE-GROUP-NAME> #use your own name for this variable
ACR_NAME=<acrname> #use your own name for this variable

#Creates the resource group that will store the ACR
az group create --name $ACR_RG_NAME --location <location>

#Creates the ACR in the resource group that was created earlier
az acr create --resource-group $ACR_RG_NAME --name $ACR_NAME --sku Basic
```
