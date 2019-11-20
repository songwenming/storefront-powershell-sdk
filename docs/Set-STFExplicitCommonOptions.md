#Set-STFExplicitCommonOptions
Set the ExplicitCommon protocol options
##Syntax
```
```
##Detailed Description
Set the ExplicitCommon Authentication service protocol options.
##Related Commands
*[Get-STFExplicitCommonOptions](Get-STFExplicitCommonOptions)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.String[]
Parameter Domains: The .NET 'System.String' reference type
###System.String
Parameter DefaultDomain: The .NET 'System.String' reference type
###System.Boolean
Parameter HideDomainField: The .NET 'System.Boolean' value type
###Citrix.StoreFront.Model.Authentication.PasswordChange
Parameter AllowUserPasswordChange: The .NET 'Citrix.StoreFront.Model.Authentication.PasswordChange' value type
###Citrix.StoreFront.Model.Authentication.PasswordExpiryWarning
Parameter ShowPasswordExpiryWarning: The .NET 'Citrix.StoreFront.Model.Authentication.PasswordExpiryWarning' value type
###System.Int32
Parameter PasswordExpiryWarningPeriod: The .NET 'System.Int32' value type
###System.Boolean
Parameter AllowZeroLengthPassword: The .NET 'System.Boolean' value type
##Return Values
##Examples
###EXAMPLE 1 Set the ExplicitCommon protocol options
```
Set-STFExplicitCommonOptions -AuthenticationService $authentication -Domains @("Alpha","Beta","Capa") -DefaultDomain Alpha -HideDomainField $true -AllowChangePassword Always -ShowPasswordExpiryWarning Windows -PasswordExpiryWarningPeriod 10
```
REMARKS

Sets the ExplicitCommon options on the only configured authentication service.
