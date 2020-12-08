---
title: "Update mailFolder"
description: "Update the properties of a mailFolder object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update mailFolder
Namespace: microsoft.graph

Update the properties of a [mailFolder](../resources/mailfolder.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mailFolders/{mailFolderId}
PATCH /users/{usersId}/mailFolders/{mailFolderId}/childFolders/{mailFolderId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mailFolder](../resources/mailfolder.md) object.

The following table shows the properties that are required when you update the [mailFolder](../resources/mailfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|childFolderCount|Int32|**TODO: Add Description**|
|unreadItemCount|Int32|**TODO: Add Description**|
|totalItemCount|Int32|**TODO: Add Description**|
|wellKnownName|String|**TODO: Add Description**|
|isHidden|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [mailFolder](../resources/mailfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mailFolders/{mailFolderId}
Content-Type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.mailFolder",
  "displayName": "String",
  "parentFolderId": "String",
  "childFolderCount": "Integer",
  "unreadItemCount": "Integer",
  "totalItemCount": "Integer",
  "wellKnownName": "String",
  "isHidden": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mailFolder",
  "displayName": "String",
  "parentFolderId": "String",
  "childFolderCount": "Integer",
  "unreadItemCount": "Integer",
  "totalItemCount": "Integer",
  "wellKnownName": "String",
  "isHidden": "Boolean",
  "id": "6a0d9272-9272-6a0d-7292-0d6a72920d6a"
}
```

