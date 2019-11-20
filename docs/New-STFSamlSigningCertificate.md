#New-STFSamlSigningCertificate
Create a new request signing certificate to be used by the SAML Service Provider
##Syntax
```
```
##Detailed Description
Create a new request signing certificate to be used by SAML Service Provider, fpr the specified authentication service
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.String
Parameter SubjectName: The .NET 'System.String' reference type
##Return Values
##Examples
###EXAMPLE 1 Create a new request signing certificate to be used by the SAML Service Provider.
```
New-STFSamlSigningCertificate -AuthenticationService $authentication -SubjectName Signing
```
REMARKS

Create a new request signing certificate, with subject name 'Signing', to be used by the SAML Service Provider in the
specified authentication service.
