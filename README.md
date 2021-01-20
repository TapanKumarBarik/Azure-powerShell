https://docs.microsoft.com/en-us/powershell/azure/get-started-azureps?view=azps-5.4.0#code-try-2


# To check the PowerShell version 
```python
$PSVersionTable.PSVersion
```

![Alt text](https://github.com/TapanKumarBarik/Azure-powerShell/blob/main/Screenshot%20(42).png)

# Install Az modules on PowerShell
```python
Install-Module -Name Az -AllowClobber -Force
```
AllowClobber for installing more than 2 versions of powershell

# To get the available versions of powershell installed 
```python
 Get-InstalledModule -Name Az -AllVersions | Select-Object Name,Version
 ```
 ![Alt text](https://github.com/TapanKumarBarik/Azure-powerShell/blob/main/Screenshot%20(43).png)
 
 # LOGIN
 ```python
 Connect-AzAccount
 ```
 ## To get all the vm running in my subscription 
 ```python 
 Get-AzVM
 ```
 https://docs.microsoft.com/en-us/powershell/module/az.compute/get-azvm?view=azps-5.4.0
 
 ## get webApps
 ```python
 Get-AzWebApp
 ```
 # Get all the subscription
 ```python
 Get-AzSubscription
 ```
 ## 
