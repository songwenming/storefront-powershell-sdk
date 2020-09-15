#Set-STFDesktopApplianceService
Configure a Desktop Appliance site
##Syntax
```
```
##Detailed Description
Configure options on the supplied Desktop Appliance site.
##Related Commands
*[Add-STFDesktopApplianceService](Add-STFDesktopApplianceService)
*[Remove-STFDesktopApplianceService](Remove-STFDesktopApplianceService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.DesktopAppliance.DesktopApplianceService
Parameter DesktopApplianceService: A .NET class representing the configuration of a StoreFront Desktop Appliance service
###System.Management.Automation.SwitchParameter
Parameter MultiDesktop: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter EnableExplicit: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter EnableSmartCard: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter EnableEmbeddedSmartcardSSO: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
###DesktopApplianceService
A .NET class representing the configuration of a StoreFront Desktop Appliance service
##Examples
###EXAMPLE 1 Configure Desktop Appliance site
```
Set-STFDesktopApplianceService -DesktopApplianceService $appliance -MultiDesktop:$false
```
REMARKS

Turn off multi-desktops on the only configured Desktop Appliance site.
