# ConversationThread: Reply


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Groups/<Id>/Threads/<Id>/Reply
POST /me/JoinedGroups/<Id>/Threads/<Id>/Reply
POST /Users/<Id>/JoinedGroups/<Id>/Threads/<Id>/Reply

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
|Post|Post||

### Response
If successful, this method returns `200, OK` response code. It does not return anything in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/Groups/<Id>/Threads/<Id>/Reply
Content-type: application/json
Content-length: 1432

{
  "Post": {
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
    "ConversationThreadId": "ConversationThreadId-value",
    "NewParticipants": [
      {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      }
    ],
    "ConversationId": "ConversationId-value",
    "CreatedDateTime": "datetime-value",
    "LastModifiedDateTime": "datetime-value",
    "ChangeKey": "ChangeKey-value",
    "Categories": [
      "Categories-value"
    ],
    "Id": "Id-value",
    "InReplyTo": {
    },
    "Attachments": [
      {
        "LastModifiedDateTime": "datetime-value",
        "Name": "Name-value",
        "ContentType": "ContentType-value",
        "Size": 99,
        "IsInline": true,
        "Id": "Id-value"
      }
    ],
    "SingleValueExtendedProperties": [
      {
        "Value": "Value-value",
        "PropertyId": "PropertyId-value"
      }
    ],
    "MultiValueExtendedProperties": [
      {
        "Value": [
          "Value-value"
        ],
        "PropertyId": "PropertyId-value"
      }
    ]
  }
}
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
  "description": "ConversationThread: Reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->