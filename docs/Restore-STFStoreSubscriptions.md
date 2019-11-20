#Restore-STFStoreSubscriptions
Restore subscriptions to given Store
##Syntax
```
Restore-STFStoreSubscriptions [-FilePath] <String> [-StoreService] <StoreService> [-FilePath] <String> [<CommonParameters>]
```
##Detailed Description
Restore user subscriptions to a Store from a text file in the correct csv format.
##Related Commands
*[Export-STFStoreSubscriptions](Export-STFStoreSubscriptions)
*[Import-STFStoreSubscriptions](Import-STFStoreSubscriptions)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.String
Parameter FilePath: The .NET 'System.String' reference type
###System.Int32
Parameter ChunkSize: The .NET 'System.Int32' value type
##Return Values
##Notes
The cmdlet replaces the all of the existing data with what is contained in the file.
##Examples
###EXAMPLE 1 Restore subscriptions
```
Restore-STFStoreSubscriptions -Store $store -FilePath "$env:userprofile\desktop\Export.txt"
```
REMARKS

Restore subscriptions into the only configured Store.
