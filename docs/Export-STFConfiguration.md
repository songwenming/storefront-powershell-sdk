#Export-STFConfiguration
Exports a zip file containing configuration elements that form a Citrix StoreFront deployment. This zip file may be unencrypted in the form of a '.zip' file or encrypted in the form of a '.ctxzip'.
##Syntax
```
```
##Detailed Description
Exports a zip file containing configuration elements that form a Citrix StoreFront deployment. This zip file may be unencrypted in the form of a '.zip' file or encrypted in the form of a '.ctxzip'.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter TargetFolder: The .NET 'System.String' reference type
###System.String
Parameter ZipFileName: The .NET 'System.String' reference type
###System.Management.Automation.PSCredential
Parameter Credential: The .NET 'System.Management.Automation.PSCredential' reference type
###System.Management.Automation.SwitchParameter
Parameter Force: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Management.Automation.SwitchParameter
Parameter NoEncryption: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Examples
###EXAMPLE 1 Basic Config Export
```
```
REMARKS

This example creates an unencrypted '.zip' file at '$env:userprofile\desktop\' called ConfigBackup.

```
```
REMARKS

This example creates an encrypted .ctxzip file as above using a pre-defined PSCredential object.
Example PSCredential:
$User = Any non empty string will suffice here. The exported configuration is secured by only using the $Password.
$Password = 'Secret'
$Password = $Password | ConvertTo-SecureString -asPlainText -Force
$CredObject = New-Object System.Management.Automation.PSCredential($User,$Password)
Create a PowerShell credential object containing a username and password for symmetric encryption and decryption of
configuration backup archives. PowerShell credential objects store passwords as secure strings in memory.
The user is irrelevant but mandatory to create a PowerShell credential object. The example code uses the currently
logged in user.
The password is used for symmetric encryption/decryption of the backup archive. NOTE: The password DOES NOT need to
match the user's password to create a valid credential object.
