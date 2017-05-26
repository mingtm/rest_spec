# List Threads

Retrieve a list of conversationthread objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /Groups/<Id>/Threads
GET /me/JoinedGroups/<Id>/Threads
GET /Users/<Id>/JoinedGroups/<Id>/Threads
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
If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/beta/Groups/<Id>/Threads
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ConversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "ToRecipients": [
        {
          "EmailAddress": {
            "Name": "Name-value",
            "Address": "Address-value"
          }
        }
      ],
      "Topic": "Topic-value",
      "HasAttachments": true,
      "LastDeliveredDateTime": "datetime-value",
      "UniqueSenders": [
        "UniqueSenders-value"
      ],
      "CcRecipients": [
        {
          "EmailAddress": {
            "Name": "Name-value",
            "Address": "Address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List Threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->