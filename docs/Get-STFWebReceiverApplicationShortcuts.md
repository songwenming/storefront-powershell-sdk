#Get-STFWebReceiverApplicationShortcuts
Get the WebReceiver application shortcuts
##Syntax
```
```
##Detailed Description
Get the WebReceiver application shortcuts.
##Related Commands
*[Set-STFWebReceiverApplicationShortcuts](Set-STFWebReceiverApplicationShortcuts)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###AppShortcutsServer
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.AppShortcutsServer' reference type
##Examples
###EXAMPLE 1 Get WebReceiver Application Shortcuts
```
Get-STFWebReceiverApplicationShortcuts -WebReceiverService $receiver
```
REMARKS

Get the WebReceiver application shortcuts of the only configured WebReceiver.
OUTPUT
```
TrustedUrls                 : {http://mycompany.com/}
GatewayUrls                 : {https://mycompanygateway.com/}
```