﻿# defaultManagedAppConfiguration resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Configuration used to deliver a set of custom settings as-is to all users not targeted by a TargetedManagedAppConfiguration type configuration

Inherits from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)

## Methods
|Method|Return Type|Description|
|---|---|---|
|[List defaultManagedAppConfigurations](../api/intune_mam_defaultmanagedappconfiguration_list.md)|[defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md) collection|List properties and relationships of the [defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md) objects.|
|[Get defaultManagedAppConfiguration](../api/intune_mam_defaultmanagedappconfiguration_get.md)|[defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md)|Read properties and relationships of the [defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md) object.|
|[Create defaultManagedAppConfiguration](../api/intune_mam_defaultmanagedappconfiguration_create.md)|[defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md)|Create a new [defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md) object.|
|[Delete defaultManagedAppConfiguration](../api/intune_mam_defaultmanagedappconfiguration_delete.md)|None|Deletes a [defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md).|
|[Update defaultManagedAppConfiguration](../api/intune_mam_defaultmanagedappconfiguration_update.md)|[defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md)|Update the properties of a [defaultManagedAppConfiguration](../resources/intune_mam_defaultmanagedappconfiguration.md) object.|
|[List mobileAppIdentifierDeployments](../api/intune_mam_defaultmanagedappconfiguration_list_mobileappidentifierdeployment.md)|[mobileAppIdentifierDeployment](../resources/intune_mam_mobileappidentifierdeployment.md) collection|Get the mobileAppIdentifierDeployments from the mobileAppIdentifierDeployments navigation property.|
|[Get managedAppPolicyDeploymentSummary](../api/intune_mam_defaultmanagedappconfiguration_get_managedapppolicydeploymentsummary.md)|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Get the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) from the deploymentSummary navigation property.|

## Properties
|Property|Type|Description|
|---|---|---|
|displayName|String|Policy display name. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|String|The policy's description. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedTime|DateTimeOffset|Last time the policy was modified. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|deployedAppCount|Int32|Count of apps to which the current policy is deployed. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|String|Key of the entity. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|version|String|Version of the entity. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|customSettings|[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection|A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|mobileAppIdentifierDeployments|[mobileAppIdentifierDeployment](../resources/intune_mam_mobileappidentifierdeployment.md) collection|List of apps to which the policy is deployed. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Navigation property to deployment summary of the configuration. Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultManagedAppConfiguration"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.defaultManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "lastModifiedTime": "String (timestamp)",
  "deployedAppCount": 1024,
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



