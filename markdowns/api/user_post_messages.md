# Create Message

Use this API to create a new Message.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Messages
POST /Users/<Id>/Messages

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Message](../resources/message.md) object.


### Response
If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/Messages
Content-type: application/json
Content-length: 272

{
  "ReceivedDateTime": "datetime-value",
  "SentDateTime": "datetime-value",
  "HasAttachments": true,
  "InternetMessageId": "InternetMessageId-value",
  "Subject": "Subject-value",
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  }
}
```
In the request body, supply a JSON representation of [Message](../resources/message.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

{
  "ReceivedDateTime": "datetime-value",
  "SentDateTime": "datetime-value",
  "HasAttachments": true,
  "InternetMessageId": "InternetMessageId-value",
  "Subject": "Subject-value",
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->