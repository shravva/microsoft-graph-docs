---
title: "Update educationAssignmentDefaults"
description: "Update the properties of an educationAssignmentDefaults object."
author: "dipakboyed"
localization_priority: Normal
ms.prod: "education"
doc_type: apiPageType
---

# Update educationAssignmentDefaults
Namespace: microsoft.graph

Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object. Only Teachers can update these settings.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account) |  EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite  |
|Delegated (personal Microsoft account) |  Not supported.  |
|Application | Not supported. |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentDefaults
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply the values for relevant fields of the [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object that should be updated. Existing properties that are not included in the request body will maintain their previous values. For best performance, don't include existing values that haven't changed.

|Property|Type|Description|
|:---|:---|:---|
|addedStudentAction|educationAddedStudentAction|class-level default behavior for handling students who are added after the assignment is published. Default value - none. Possible values are: `none`, `assignIfOpen`.|
|dueTime|TimeOfDay|class-level default value for due time field. Default value - 23:59:00|
|notificationChannelUrl|String|Default Teams channel to which notifications will be sent. Default value - null.|



## Response

If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/educationClass/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
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
  "addedStudentAction": "assignIfOpen",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

