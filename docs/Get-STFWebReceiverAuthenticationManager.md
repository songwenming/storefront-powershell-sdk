#Get-STFWebReceiverAuthenticationManager
Get the WebReceiver Authentication Manager options
##Syntax
```
```
##Detailed Description
Get the WebReceiver Authentication Manager client options.
##Related Commands
*[Set-STFWebReceiverAuthenticationManager](Set-STFWebReceiverAuthenticationManager)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###AuthManager
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.AuthManager' reference type
##Examples
###EXAMPLE 1 Get WebReceiver Authentication options
```
Get-STFWebReceiverAuthenticationManager -WebReceiverService $receiver
```
REMARKS

Get the WebReceiver Authentication Manager options of the only configured WebReceiver.
OUTPUT
```
LogoffUrl            : Authentication/Logoff
ChangeCredentialsUrl : ExplicitAuth/GetChangeCredentialForm
LoginFormTimeout     : 5
```