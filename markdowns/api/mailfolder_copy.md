# MailFolder: Copy


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/MailFolders/<Id>/Copy
POST /Users/<Id>/MailFolders/<Id>/Copy

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|DestinationId|String||

### Response
If successful, this method returns `200, OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->
```http
POST https://graph.microsoft.com/beta/me/MailFolders/<Id>/Copy
Content-type: application/json
Content-length: 44

{
  "DestinationId": "DestinationId-value"
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.MailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "DisplayName": "DisplayName-value",
  "ParentFolderId": "ParentFolderId-value",
  "ChildFolderCount": 99,
  "UnreadItemCount": 99,
  "TotalItemCount": 99,
  "WellKnownName": "WellKnownName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MailFolder: Copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->