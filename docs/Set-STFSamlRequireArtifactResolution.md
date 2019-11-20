#Set-STFSamlRequireArtifactResolution
Configure whether the SAML Artifact Resolution protocol is required for Single Signle Sign-on
##Syntax
```
```
##Detailed Description
Configure whether the SAML Artifact Resolution protocol is required for Single Signle Sign-on, for the specified authentication service
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.Boolean
Parameter Required: The .NET 'System.Boolean' value type
##Return Values
##Examples
###EXAMPLE 1 Require Artifact Resolution
```
Set-STFSamlRequire -AuthenticationService $authentication -Required $true
```
REMARKS

Configure the SAML Service Provider in the specified authentication service, to require the use of the Artifact
Resolution protocol.
