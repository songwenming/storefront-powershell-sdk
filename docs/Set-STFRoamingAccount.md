#Set-STFRoamingAccount
Set the roaming account properties
##Syntax
```
```
##Detailed Description
Configure the roaming account properties for a given Store.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.Boolean
Parameter Published: The .NET 'System.Boolean' value type
###Citrix.StoreFront.Model.Roaming.RoamingService
Parameter RoamingService: A .NET class representing the configuration of a StoreFront Roaming service
##Return Values
##Examples
###EXAMPLE 1 Set the roaming account properties to hide the Store
```
Set-STFRoamingAccount -StoreService $store -Published $false
```
REMARKS

Set the Roaming account for the only configured Store service to hide the Store from Receivers.
