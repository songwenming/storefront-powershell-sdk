#Set-STFStoreLaunchOptions
Set Store launch options
##Syntax
```
```
##Detailed Description
Set the options used by a Store when launching an application or desktop on XenApp and XenDesktop.
##Related Commands
*[Get-STFStoreLaunchOptions](Get-STFStoreLaunchOptions)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###Citrix.StoreFront.Model.Store.AddressResolutionType
Parameter AddressResolutionType: The .NET 'Citrix.StoreFront.Model.Store.AddressResolutionType' value type
###Citrix.StoreFront.Model.Store.RequestICAClientSecureChannel
Parameter RequestIcaClientSecureChannel: The .NET 'Citrix.StoreFront.Model.Store.RequestICAClientSecureChannel' value type
###System.Boolean
Parameter AllowSpecialFolderRedirection: The .NET 'System.Boolean' value type
###System.Boolean
Parameter AllowFontSmoothing: The .NET 'System.Boolean' value type
###System.Boolean
Parameter RequireLaunchReference: The .NET 'System.Boolean' value type
###System.Boolean
Parameter OverrideIcaClientName: The .NET 'System.Boolean' value type
###System.Boolean
Parameter OverlayAutoLoginCredentialsWithTicket: The .NET 'System.Boolean' value type
###System.Boolean
Parameter IgnoreClientProvidedClientAddress: The .NET 'System.Boolean' value type
###System.Boolean
Parameter SetNoLoadBiasFlag: The .NET 'System.Boolean' value type
###System.Boolean
Parameter RDPOnly: The .NET 'System.Boolean' value type
###System.String
Parameter IcaTemplateName: The .NET 'System.String' reference type
###System.String
Parameter VdaLogonDataProvider: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter Force: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Examples
###EXAMPLE 1 Set Store launch options
```
Set-STFStoreLaunchOptions $storeService -AddressResolutionType Dns -RequestIcaClientSecureChannel DetectAnyCiphers -AllowSpecialFolderRedirection $true -AllowFontSmoothing $true
```
REMARKS

Set the Store to use Dns address resolution type, Ica secure channel to DetectAnyCiphers, allow folder redirection and
font smoothing.

```
Set-STFStoreLaunchOptions -StoreService $storeService -VdaLogonDataProvider 'FASLogonDataProvider'
```
REMARKS

Set the Store to use the Federated Authentication Service Vda logon data provider during launch.
