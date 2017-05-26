# List Posts

Retrieve a list of post objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /Groups/<Id>/Threads/<Id>/Posts
GET /me/JoinedGroups/<Id>/Threads/<Id>/Posts
GET /Users/<Id>/JoinedGroups/<Id>/Threads/<Id>/Posts
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/Groups/<Id>/Threads/<Id>/Posts
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 531

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List Posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->