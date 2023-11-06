``` bash
# Create a resource group
az group create --name myResourceGroup --location EastUS

# Deploy template into resource group
az deployment group create --resource-group testrg --name rollout01 \
    --template-file azuredeploy.json  --parameters params.json \
```

```bash 
# Delete a resource group
az group delete --name ExampleResourceGroup
```
```bash
# Delete a resource
az resource delete \
  --resource-group ExampleResourceGroup \
  --name ExampleVM \
  --resource-type "Microsoft.Compute/virtualMachines"
```