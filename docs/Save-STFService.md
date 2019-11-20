#Save-STFService
Save changes to a StoreFront service
##Syntax
```
```
##Detailed Description
Save changes made to a StoreFront service in memory object.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFrontConfiguration.Interfaces.IConfigBasedFeature
Parameter Service: The .NET 'Citrix.StoreFrontConfiguration.Interfaces.IConfigBasedFeature' reference type
##Return Values
##Notes
With the exception of those commands that state they don't in the help the save action is executed implicitly on a service when executing StoreFront PowerShell against that object.
##Examples
###EXAMPLE 1 Save changes to the Store service
```
$store.Service.AllowSessionReconnect = $false
Save-STFService $store
```
REMARKS

Disable session reconnect and save the changes.
