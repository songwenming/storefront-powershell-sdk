#Unregister-STFStoreGateway
Unregister a Gateway from a Store
##Syntax
```
Unregister-STFStoreGateway [-Name] <String> [-StoreService] <StoreService> [<CommonParameters>]
Unregister-STFStoreGateway [-AllGateways] <SwitchParameter> [-StoreService] <StoreService> [<CommonParameters>]
```
##Detailed Description
Unregister a Gateway from a Store used for authentication and launch (if configured for launch)
##Related Commands
*[Register-STFStoreOptimalLaunchGateway](Register-STFStoreOptimalLaunchGateway)
*[Register-STFStoreGateway](Register-STFStoreGateway)
*[Unregister-STFStoreOptimalLaunchGateway](Unregister-STFStoreOptimalLaunchGateway)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Common.ICommonGateway
Parameter Gateway: The .NET 'Citrix.StoreFront.Model.Common.ICommonGateway' reference type
###System.String
Parameter Name: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter AllGateways: The .NET 'System.Management.Automation.SwitchParameter' value type
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
##Return Values
##Examples
###EXAMPLE 1 Remove Gateway by name
```
UnRegister-STFStoreGateway -StoreService $storeService -Name Netscaler10x
```
REMARKS

Remove the Gateway object by name

```
$gateway = Get-STFRoamingGateway -Name Netscaler10x
UnRegister-STFStoreGateway -StoreService $storeService -Gateway $gateway
```
REMARKS

Remove the Gateway object Netscaler10x from the only Store
