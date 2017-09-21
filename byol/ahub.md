# Steps 
1. Create VM with AHUB
2. Query VM Info
```powershell	
	Get-AzureRmVM -ResourceGroupName IGNITE17 -Name ProdWin16hub
``` 

3. Check Bill statement: Charges are correct?
4. List all VMs with AHUB
```powershell
$vms = Get-AzureRMVM 
foreach ($vm in $vms) {"VM Name: " + $vm.Name, "   AHUB: "+ $vm.LicenseType}
 ``` 

