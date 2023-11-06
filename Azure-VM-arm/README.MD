``` bash
# Create a resource group
az group create --name myResourceGroup --location EastUS

# Deploy template into resource group
az deployment group create --resource-group testrg --name rollout01 \
    --template-file azuredeploy.json  --parameters params.json \
```

