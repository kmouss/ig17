# Steps 
```powershell	
	Set-AzureRmContext -SubscriptionName "Visual Studio Ultimate with MSDN"
	New-AzureRmResourceGroup -Name Autoscale -Location "South Central US"
	New-AzureRmResourceGroupDeployment -Name autos1 -ResourceGroupName Autoscale -TemplateUri https://raw.githubusercontent.com/kmouss/ig17/demos/autoscale/azuredeploy.json
``` 

post deployment

1. http://13.66.36.158:9000/
2. http://13.66.36.158:9000/do_work
3. http://13.66.36.158:9000/stop_work
