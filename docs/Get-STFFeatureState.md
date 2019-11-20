#Get-STFFeatureState
Gets the registered FeatureState object
##Syntax
```
```
##Detailed Description
Gets the registered FeatureState object
##Related Commands
*[Add-STFFeatureState](Add-STFFeatureState)
*[Get-STFFeatureStateNames](Get-STFFeatureStateNames)
*[New-STFFeatureState](New-STFFeatureState)
*[New-STFFeatureStateProperty](New-STFFeatureStateProperty)
*[Remove-STFFeatureState](Remove-STFFeatureState)
*[Clear-STFFeatureStates](Clear-STFFeatureStates)
*[Reset-STFFeatureData](Reset-STFFeatureData)
*[Set-STFFeatureState](Set-STFFeatureState)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
##Return Values
###FeatureState
The .NET 'Citrix.DeliveryServices.Framework.FeatureToggle.FeatureState' reference type
##Examples
###EXAMPLE 1 Get FeatureState object
```
```
REMARKS

Gets FeatureState object identified by feature1
OUTPUT
```
----                       --------- ----------                        
Feature1                    True      {Property1, Property2}
```
###EXAMPLE 2 Get FeatureState objects
```
```
REMARKS

Gets a list of registred FeatureState objects
OUTPUT
```
----                       --------- ----------                        
Feature1                    True      {Property1, Property2}              
Feature2                    True      {}
```