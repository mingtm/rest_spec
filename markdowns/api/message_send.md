# Message: Send


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Messages/<Id>/Send
POST /Users/<Id>/Messages/<Id>/Send
POST /me/MailFolders/<Id>/Messages/<Id>/Send

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body

### Response
If successful, this method returns `200, OK` response code. It does not return anything in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/beta/me/Messages/<Id>/Send
```

##### Response
Here is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Message: Send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->