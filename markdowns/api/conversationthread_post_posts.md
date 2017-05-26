# Create Post

Use this API to create a new Post.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Groups/<Id>/Threads/<Id>/Posts
POST /me/JoinedGroups/<Id>/Threads/<Id>/Posts
POST /Users/<Id>/JoinedGroups/<Id>/Threads/<Id>/Posts

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Post](../resources/post.md) object.


### Response
If successful, this method returns `201, Created` response code and [Post](../resources/post.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_post_from_conversationthread"
}-->
```http
POST https://graph.microsoft.com/beta/Groups/<Id>/Threads/<Id>/Posts
Content-type: application/json
Content-length: 426

{
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "ReceivedDateTime": "datetime-value",
  "HasAttachments": true,
  "From": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "Sender": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "ConversationThreadId": "ConversationThreadId-value"
}
```
In the request body, supply a JSON representation of [Post](../resources/post.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Post"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 426

{
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "ReceivedDateTime": "datetime-value",
  "HasAttachments": true,
  "From": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "Sender": {
    "EmailAddress": {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  },
  "ConversationThreadId": "ConversationThreadId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->