---
title: "Remove educationCategory"
description: "Remove an existing educationCategory from this educationAssignment."
ms.localizationpriority: medium
author: "dipakboyed"
ms.subservice: "education"
ms.collection: "education"
doc_type: apiPageType
---

# Remove educationCategory

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md). Only teachers can perform this operation.

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions
Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "educationassignment_remove_category" } -->
[!INCLUDE [permissions-table](../includes/permissions/educationassignment-remove-category-permissions.md)]

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## Request headers
| Header       | Value |
|:---------------|:--------|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body
Don't supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Example
### Request
The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "remove_educationcategory_from_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/e98aaae1-7c98-4e65-bb62-1994fe410552/categories/39e3d9dc-7244-42d7-8b4d-1071aae5eb41/$ref
```

### Response
The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


