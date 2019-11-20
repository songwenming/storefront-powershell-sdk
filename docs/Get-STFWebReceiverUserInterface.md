#Get-STFWebReceiverUserInterface
Get the WebReceiver User Interface options
##Syntax
```
```
##Detailed Description
Get the WebReceiver User Interface client options.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###UserInterface
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.UserInterface' reference type
##Examples
###EXAMPLE 1 Get WebReceiver User Interface options
```
Get-STFWebReceiverUserInterface -WebReceiverService $receiver
```
REMARKS

Get the WebReceiver User Interface options of the only configured WebReceiver.
OUTPUT
```
MultiClickTimeout     : 3
EnableAppsFolderView  : True
WorkspaceControl      : Enabled              : True
                        AutoReconnectAtLogon : True
                        LogoffAction         : Disconnect
                        ShowReconnectButton  : True
                        ShowDisconnectButton : True
ReceiverConfiguration : Enabled     : True
                        DownloadUrl : ServiceRecord/GetDocument/receiverconfig.cr
AppShortcuts          : Enabled               : False
                        AllowSessionReconnect : False
UIViews               : ShowAppsView     : True
                        ShowDesktopsView : True
                        DefaultView      : Auto
```