---
title: "Get mailFolder"
description: "Read the properties and relationships of a mailFolder object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get mailFolder
Namespace: microsoft.graph

Read the properties and relationships of a [mailFolder](../resources/mailfolder.md) object.

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
GET /users/{usersId}/mailFolders/{mailFolderId}
GET /users/{usersId}/mailFolders/{mailFolderId}/childFolders/{mailFolderId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mailFolders/{mailFolderId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OutlookServices.mailFolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.OutlookServices.mailFolder",
    "displayName": "String",
    "parentFolderId": "String",
    "childFolderCount": "Integer",
    "unreadItemCount": "Integer",
    "totalItemCount": "Integer",
    "wellKnownName": "String",
    "isHidden": "Boolean",
    "id": "6a0d9272-9272-6a0d-7292-0d6a72920d6a"
  }
}
```

