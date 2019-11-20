#Set-STFStoreFarm
Set the details of an exiting farm
##Syntax
```
Set-STFStoreFarm [-StoreService] <StoreService> [-FarmName] <String> [[-FarmType] <XenApp | XenDesktop | AppController | VDIinaBox | Store>] [[-Servers] <String[]>] [[-ServiceUrls] <String[]>] [[-Port] <Int32>] [[-TransportType] <HTTP | HTTPS | SSL>] [[-SSLRelayPort] <Int32>] [[-LoadBalance] <Boolean>] [[-AllFailedBypassDuration] <Int32>] [[-BypassDuration] <Int32>] [[-TicketTimeToLive] <Int32>] [[-RadeTicketTimeToLive] <Int32>] [[-MaxFailedServersPerRequest] <Int32>] [[-Zones] <String[]>] [[-Product] <String>] [[-RestrictPoPs] <String>] [[-FarmGuid] <String>] [[-PassThru] <SwitchParameter>] [<CommonParameters>]
```
##Detailed Description
Set the details of an existing farm.
##Related Commands
*[Add-STFStoreFarm](Add-STFStoreFarm)
*[Remove-STFStoreFarm](Remove-STFStoreFarm)
*[Get-STFStoreFarm](Get-STFStoreFarm)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.Farm
Parameter Farm: A .NET class representing the configuration of a Farm in StoreFront Store service
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.String
Parameter FarmName: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.FarmType
Parameter FarmType: The .NET 'Citrix.StoreFront.Model.Store.FarmType' value type
###System.String[]
Parameter Servers: The .NET 'System.String' reference type
###System.String[]
Parameter ServiceUrls: The .NET 'System.String' reference type
###System.Int32
Parameter Port: The .NET 'System.Int32' value type
###Citrix.StoreFront.Model.Store.TransportType
Parameter TransportType: The .NET 'Citrix.StoreFront.Model.Store.TransportType' value type
###System.Int32
Parameter SSLRelayPort: The .NET 'System.Int32' value type
###System.Boolean
Parameter LoadBalance: The .NET 'System.Boolean' value type
###System.Int32
Parameter AllFailedBypassDuration: The .NET 'System.Int32' value type
###System.Int32
Parameter BypassDuration: The .NET 'System.Int32' value type
###System.Int32
Parameter TicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter RadeTicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter MaxFailedServersPerRequest: The .NET 'System.Int32' value type
###System.String[]
Parameter Zones: The .NET 'System.String' reference type
###System.String
Parameter Product: The .NET 'System.String' reference type
###System.String
Parameter RestrictPoPs: The .NET 'System.String' reference type
###System.String
Parameter FarmGuid: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Examples
###EXAMPLE 1 Reconfigure existing farm
```
$farm = Get-STFStoreFarm -StoreService $storeService
Set-STFStoreFarm $farm -FarmType XenDesktop -Port 80 -TransportType HTTP -Servers Xen1,Xen2
```
REMARKS

Reconfigure the settings on an existing farm.
