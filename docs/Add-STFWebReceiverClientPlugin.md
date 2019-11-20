#Add-STFWebReceiverClientPlugin
Add a WebReceiver client plug-in
##Syntax
```
```
##Detailed Description
Add WebReceiver script and branding customizations.
##Related Commands
*[Clear-STFWebReceiverClientPlugin](Clear-STFWebReceiverClientPlugin)
*[Get-STFWebReceiverClientPlugin](Get-STFWebReceiverClientPlugin)
*[New-STFWebReceiverClientPlugin](New-STFWebReceiverClientPlugin)
*[Remove-STFWebReceiverClientPlugin](Remove-STFWebReceiverClientPlugin)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
###Citrix.StoreFront.Model.ReceiverForWeb.ClientPlugin[]
Parameter ClientPlugin: The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.ClientPlugin' reference type
##Return Values
##Examples
###EXAMPLE 1 Add a client plugin
```
$plugin = New-STFWebReceiverClientPlugin -Name "NetScaler" `
-Source "/plugins/netscalar/script1.js" `
-Scripts @("/plugins/netscalar/script2.js", "/plugins/netscalar/script1.js") `
-Styles @("/plugins/netscalar/script2.css","/plugins/netscalar/script1.css") `
-Parameters @{"param1" = "value1";"param2" = "value2"}
Add-STFWebReceiverClientPlugin -WebReceiverService $webReceiver -ClientPlugin $plugin
```
REMARKS

Creates and adds a client plug-in to the only WebReceiver service.
