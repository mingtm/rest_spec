# Message: CreateReply


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Messages/<Id>/CreateReply
POST /Users/<Id>/Messages/<Id>/CreateReply
POST /me/MailFolders/<Id>/Messages/<Id>/CreateReply

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
|Message|Message||
|Comment|String||

### Response
If successful, this method returns `200, OK` response code and [Message](../resources/message.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/beta/me/Messages/<Id>/CreateReply
Content-type: application/json
Content-length: 2905

{
  "Message": {
    "ReceivedDateTime": "datetime-value",
    "SentDateTime": "datetime-value",
    "HasAttachments": true,
    "InternetMessageId": "InternetMessageId-value",
    "Subject": "Subject-value",
    "Body": {
      "ContentType": "ContentType-value",
      "Content": "Content-value"
    },
    "BodyPreview": "BodyPreview-value",
    "Importance": "Importance-value",
    "ParentFolderId": "ParentFolderId-value",
    "Sender": {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    },
    "From": {
      "EmailAddress": {
        "Name": "Name-value",
        "Address": "Address-value"
      }
    },
    "ToRecipients": [
      {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      }
    ],
    "CcRecipients": [
      {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      }
    ],
    "BccRecipients": [
      {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      }
    ],
    "ReplyTo": [
      {
        "EmailAddress": {
          "Name": "Name-value",
          "Address": "Address-value"
        }
      }
    ],
    "ConversationId": "ConversationId-value",
    "ConversationIndex": "ConversationIndex-value",
    "UniqueBody": {
      "ContentType": "ContentType-value",
      "Content": "Content-value"
    },
    "IsDeliveryReceiptRequested": true,
    "IsReadReceiptRequested": true,
    "IsRead": true,
    "IsDraft": true,
    "WebLink": "WebLink-value",
    "InferenceClassification": "InferenceClassification-value",
    "UnsubscribeData": [
      "UnsubscribeData-value"
    ],
    "UnsubscribeEnabled": true,
    "Flag": {
      "CompletedDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "DueDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "StartDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "FlagStatus": "FlagStatus-value"
    },
    "CreatedDateTime": "datetime-value",
    "LastModifiedDateTime": "datetime-value",
    "ChangeKey": "ChangeKey-value",
    "Categories": [
      "Categories-value"
    ],
    "Id": "Id-value",
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
  },
  "Comment": "Comment-value"
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Message"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Message: CreateReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->