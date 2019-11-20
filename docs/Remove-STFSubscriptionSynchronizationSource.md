#Remove-STFSubscriptionSynchronizationSource
Remove a synchronization source
##Syntax
```
Remove-STFSubscriptionSynchronizationSource [-FriendlyName] <String> [[-PassThru] <SwitchParameter>] [<CommonParameters>]
```
##Detailed Description
Remove a remote StoreFront synchronization source, self service application and desktop subscriptions are pulled from.
##Related Commands
*[Get-STFSubscriptionSynchronizationSource](Get-STFSubscriptionSynchronizationSource)
*[Clear-STFSubscriptionSynchronizationSource](Clear-STFSubscriptionSynchronizationSource)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter RemoteStoreFrontAddress: The .NET 'System.String' reference type
###System.String
Parameter FriendlyName: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Notes
Restarts the Citrix Subscription Store Service to read new settings.
The name of the Store on the remote StoreFront must match that on the local StoreFront group for subscriptions to correctly update.Permissions must be configured using the Grant-STFSubscriptionSynchronization cmdlet on the remote StoreFront.
##Examples
###EXAMPLE 1 Remove a named source
```
```
REMARKS

Removes the source named APACGroup.

```
```
REMARKS

Remove the synchronization source with the address apac.example.com.
