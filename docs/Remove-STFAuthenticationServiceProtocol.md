#Remove-STFAuthenticationServiceProtocol
Remove a protocol from the Authentication service
##Syntax
```
```
##Detailed Description
Remove a protocol from the specified Authentication service.
##Related Commands
*[Get-STFAuthenticationProtocolsAvailable](Get-STFAuthenticationProtocolsAvailable)
*[Enable-STFAuthenticationServiceProtocol](Enable-STFAuthenticationServiceProtocol)
*[Disable-STFAuthenticationServiceProtocol](Disable-STFAuthenticationServiceProtocol)
*[Add-STFAuthenticationServiceProtocol](Add-STFAuthenticationServiceProtocol)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String[]
Parameter Name: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
##Return Values
##Examples
###EXAMPLE 1 Remove the HttpBasic authentication protocol
```
Remove-STFAuthenticationServiceProtocol -AuthenticationService $authentication -Name HttpBasic
```
REMARKS

Removes the HttpBasic authentication protocol from the $authentication service
