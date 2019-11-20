#Update-STFSamlIdPFromMetadata
Update the SAML Identity Provider configuration from metadata.
##Syntax
```
```
##Detailed Description
Update the SAML Identity Provider configuration from metadata, for the specified authentication service
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.String
Parameter Url: The .NET 'System.String' reference type
###System.String
Parameter FilePath: The .NET 'System.String' reference type
##Return Values
##Examples
###EXAMPLE 1 Update the SAML IdentityProvider configuration from a metadata url
```
Update-STFSamlIdPFromMetadata -AuthenticationService $authentication -Url 'https://adfs.host.com/FederationMetadata/2007-06/FederationMetadata.xml'
```
REMARKS

Get the Identity Provider configuration from the specified ADFS metadata Url
