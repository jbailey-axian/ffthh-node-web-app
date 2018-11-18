To deploy this into Azure you need to:
1) Install the Azure CLI
2) Login to Azure using the CLI (az login)
3) Choose the correct subscription (az account list, az account show, az account set -s "Azure Sponsor Sandbox")
4) Create a resource group: az group create --name ffthh-jan-[your-initials] --location "West US 2"
5) Deploy our ARM template:
az group deployment create --resource-group ffthh-jan-[your-initials] --template-file environment\arm-template.json