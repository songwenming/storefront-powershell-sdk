#New-STFRoamingGateway
Create a new in memory Gateway that can be added and used for remote access and authentication.
##Syntax
```
```
##Detailed Description
Create a new Gateway that can be added to the global gateway list. Gateways for remote access and authentication are added to Stores from the globally managed list.
##Related Commands
*[Get-STFRoamingGateway](Get-STFRoamingGateway)
*[Remove-STFRoamingGateway](Remove-STFRoamingGateway)
*[Set-STFRoamingGateway](Set-STFRoamingGateway)
*[Add-STFRoamingGateway](Add-STFRoamingGateway)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Roaming.GatewayLogonType
Parameter LogonType: The .NET 'Citrix.StoreFront.Model.Roaming.GatewayLogonType' value type
###Citrix.StoreFront.Model.Roaming.GatewayLogonType
Parameter SmartCardFallbackLogonType: The .NET 'Citrix.StoreFront.Model.Roaming.GatewayLogonType' value type
###Citrix.StoreFront.Model.Roaming.GatewayVersion
Parameter Version: The .NET 'Citrix.StoreFront.Model.Roaming.GatewayVersion' value type
###System.Uri
Parameter GatewayUrl: The .NET 'System.Uri' reference type
###System.Uri
Parameter CallbackUrl: The .NET 'System.Uri' reference type
###System.Management.Automation.SwitchParameter
Parameter SessionReliability: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter RequestTicketTwoSTAs: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.String
Parameter SubnetIPAddress: The .NET 'System.String' reference type
###System.Uri[]
Parameter SecureTicketAuthorityUrls: The .NET 'System.Uri' reference type
###System.Management.Automation.SwitchParameter
Parameter StasUseLoadBalancing: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.TimeSpan
Parameter StasBypassDuration: The .NET 'System.TimeSpan' value type
###System.Uri
Parameter GslbUrl: The .NET 'System.Uri' reference type
##Return Values
###RoamingGateway
The .NET 'Citrix.StoreFront.Model.Roaming.RoamingGateway' reference type
##Examples
###EXAMPLE 1 Add Version 10x Gateway
```
Add-STFRoamingGateway $gw
```
REMARKS

Add a version 10 or greater Gateway.

```
```
REMARKS

Add a version 9 Gateway.
