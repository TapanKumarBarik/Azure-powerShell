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
 ## Case : More than 1 subscripton
 
 ### 1 : get all the available subscription
 ```python
 Get-AzSubscription
 ```
 
  ### 2: set the context variable of the subscription you want to use
 ```python
 $context=Get-Subscription -SubscriptionId <Subscription id>
 
 ```
  
  ### 3: set azure context
 ```python
 Set-AzContext $context
 
 ```
 
