# Web-API-Dock-Image-ACR-Github-Actions

Create necessary resources in the Azure
```
#Optional - This command is only necessary if you're using a local terminal
az login

# Resource Group
ACR_RG_NAME="acrTest-RG" #use your own name for this variable
ACR_NAME="eastcanadadevtestacr" #use your own name for this variable

#Creates the resource group that will store the ACR
az group create --name $ACR_RG_NAME --location canadaeast

#Creates the ACR in the resource group that was created earlier
az acr create --resource-group myResourceGroup --name $ACR_NAME --sku Basic
```
