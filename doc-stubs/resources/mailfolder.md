---
title: "mailFolder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mailFolder resource type

Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List mailFolders](../api/mailfolder-list.md)|[mailFolder](../resources/mailfolder.md) collection|Get a list of the [mailFolder](../resources/mailfolder.md) objects and their properties.|
|[Create mailFolder](../api/mailfolder-create.md)|[mailFolder](../resources/mailfolder.md)|Create a new [mailFolder](../resources/mailfolder.md) object.|
|[Get mailFolder](../api/mailfolder-get.md)|[mailFolder](../resources/mailfolder.md)|Read the properties and relationships of a [mailFolder](../resources/mailfolder.md) object.|
|[Update mailFolder](../api/mailfolder-update.md)|[mailFolder](../resources/mailfolder.md)|Update the properties of a [mailFolder](../resources/mailfolder.md) object.|
|[Delete mailFolder](../api/mailfolder-delete.md)|None|Deletes a [mailFolder](../resources/mailfolder.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childFolderCount|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isHidden|Boolean|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|totalItemCount|Int32|**TODO: Add Description**|
|unreadItemCount|Int32|**TODO: Add Description**|
|wellKnownName|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[mailFolder](../resources/mailfolder.md) collection|**TODO: Add Description**|
|messageRules|[messageRule](../resources/messagerule.md) collection|**TODO: Add Description**|
|messages|[message](../resources/message.md) collection|**TODO: Add Description**|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|userConfigurations|[userConfiguration](../resources/userconfiguration.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailFolder",
  "displayName": "String",
  "parentFolderId": "String",
  "childFolderCount": "Integer",
  "unreadItemCount": "Integer",
  "totalItemCount": "Integer",
  "wellKnownName": "String",
  "isHidden": "Boolean",
  "id": "String (identifier)"
}
```

