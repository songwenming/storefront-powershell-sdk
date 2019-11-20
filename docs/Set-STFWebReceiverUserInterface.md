#Set-STFWebReceiverUserInterface
Set the WebReceiver User Interface options
##Syntax
```
```
##Detailed Description
Set the WebReceiver User Interface client options.
##Related Commands
*[Get-STFWebReceiverUserInterface](Get-STFWebReceiverUserInterface)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
###System.Boolean
Parameter AutoLaunchDesktop: The .NET 'System.Boolean' value type
###System.Int32
Parameter MultiClickTimeout: The .NET 'System.Int32' value type
###System.Boolean
Parameter EnableAppsFolderView: The .NET 'System.Boolean' value type
###System.Boolean
Parameter ShowAppsView: The .NET 'System.Boolean' value type
###System.Boolean
Parameter ShowDesktopsView: The .NET 'System.Boolean' value type
###Citrix.StoreFront.Model.ReceiverForWeb.DefaultUIView
Parameter DefaultView: The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.DefaultUIView' value type
###System.Boolean
Parameter WorkspaceControlEnabled: The .NET 'System.Boolean' value type
###System.Boolean
Parameter WorkspaceControlAutoReconnectAtLogon: The .NET 'System.Boolean' value type
###Citrix.StoreFront.Model.ReceiverForWeb.LogoffAction
Parameter WorkspaceControlLogoffAction: The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.LogoffAction' value type
###System.Boolean
Parameter WorkspaceControlShowReconnectButton: The .NET 'System.Boolean' value type
###System.Boolean
Parameter WorkspaceControlShowDisconnectButton: The .NET 'System.Boolean' value type
###System.Boolean
Parameter ReceiverConfigurationEnabled: The .NET 'System.Boolean' value type
###System.Boolean
Parameter AppShortcutsEnabled: The .NET 'System.Boolean' value type
###System.Boolean
Parameter AppShortcutsAllowSessionReconnect: The .NET 'System.Boolean' value type
##Return Values
##Examples
###EXAMPLE 1 Set WebReceiver multi-click timeout and desktop auto launch User Interface options
```
Set-STFWebReceiverUserInterface -WebReceiverService $receiver -AutoLaunchDesktop $false -MultiClickTimeout 10
```
REMARKS

Set WebReceiver multi-click timeout to 10 seconds and disable desktop auto launch in the User Interface options.
