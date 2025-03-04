---
title: "outlookTaskFolder: permanentDelete"
description: "Permanently delete an outlook task folder and remove its items from the user's mailbox."
author: "deepakbaghel99"
ms.localizationpriority: high
ms.subservice: "outlook"
doc_type: apiPageType
---

# outlookTaskFolder: permanentDelete

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permanently delete an outlook task folder and remove its items from the user's mailbox. For more information about item retention, see [Configure Deleted Item retention and Recoverable Items quotas](/exchange/configure-deleted-item-retention-and-recoverable-items-quotas-exchange-2013-help).

>**Note:** Folders aren't placed in the Purges folder when they are permanently deleted. Permanently deleted folders are removed from the mailbox.


[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "outlooktaskfolder_permanentdelete" } -->
[!INCLUDE [permissions-table](../includes/permissions/outlooktaskfolder-permanentdelete-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/outlook/taskFolders/{outlookTaskFolderId}/permanentDelete
POST /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/permanentDelete
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|

## Request body

Don't supply a request body for this method.

## Response

If successful, this action returns a `204 No Content` response code.

## Examples

### Request

The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "outlooktaskfolderthis.permanentdelete"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/outlook/taskFolders/{outlookTaskFolderId}/permanentDelete
```


### Response

The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update checklistItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.microsoft.graph/users:
      /users/{var}/outlook/taskFolders/{var}/permanentDelete
      Uri path requires navigating into unknown object hierarchy: missing property 'taskFolders' on 'outlookUser'. Possible issues:
  	 1) Doc bug where 'taskFolders' isn't defined on the resource.
  	 2) Doc bug where 'taskFolders' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.
  	 3) Doc bug where 'outlookUser' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation."
  ]
}
-->
