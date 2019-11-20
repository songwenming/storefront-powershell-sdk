#New-STFSessionManagerTrustedIssuer
Create a new in memory SessionManagerTrustedIssuer object that represents a trusted signer of session manager assertions.
##Syntax
```
```
##Detailed Description
SessionManagerTrustedIssuers are added to the store configuration.
##Related Commands
*[Remove-STFSessionManagerTrustedIssuer](Remove-STFSessionManagerTrustedIssuer)
*[Add-STFSessionManagerTrustedIssuer](Add-STFSessionManagerTrustedIssuer)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
###System.String
Parameter Thumbprint: The .NET 'System.String' reference type
###System.String
Parameter TenantId: The .NET 'System.String' reference type
##Return Values
###SessionManagerTrustedIssuer
The .NET 'Citrix.StoreFront.Model.SessionManager.SessionManagerTrustedIssuer' reference type
##Examples
###EXAMPLE 1 Add a session manager trusted issuer to a store service.
```
$trustedIssuer = New-STFSessionManagerTrustedIssuer -Thumbprint '9ca5d6dbc06fc48cb0115d337c7b030aba56a835' -Name 'test issuer'
Add-STFSessionManagerTrustedIssuer -StoreService $storeService -SessionManagerTrustedIssuer $trustedIssuer
```
REMARKS

Add a session manager trusted issuer to a store service.
