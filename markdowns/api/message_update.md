# Update the properties of message object.

Update the properties of message object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/<objectId>/Messages/<Id>
PATCH /drive/root/createdByUser/Messages/<Id>
PATCH /users/<objectId>/RootFolder/Messages/<Id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|BccRecipients|Recipient||
|Body|ItemBody||
|BodyPreview|String||
|Categories|String||
|CcRecipients|Recipient||
|ChangeKey|String||
|ConversationId|String||
|DateTimeCreated|DateTimeOffset||
|DateTimeLastModified|DateTimeOffset||
|DateTimeReceived|DateTimeOffset||
|DateTimeSent|DateTimeOffset||
|From|Recipient||
|HasAttachments|Boolean||
|Importance|String| Possible values are: `Low`, `Normal`, `High`.|
|IsDeliveryReceiptRequested|Boolean||
|IsDraft|Boolean||
|IsRead|Boolean||
|IsReadReceiptRequested|Boolean||
|ParentFolderId|String||
|ReplyTo|Recipient||
|Sender|Recipient||
|Subject|String||
|ToRecipients|Recipient||
|UniqueBody|ItemBody||
|WebLink|String||

### Response
If successful, this method returns a `200 OK` response code and updated [Message](../resources/message.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PUT /users/<objectId>/Messages/<Id>
Content-type: application/json
Content-length: 1546
{
  "Subject": "Subject-value",
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "BodyPreview": "BodyPreview-value",
  "Importance": "Importance-value",
  "HasAttachments": true,
  "ParentFolderId": "ParentFolderId-value",
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
  "UniqueBody": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "DateTimeReceived": "datetime-value",
  "DateTimeSent": "datetime-value",
  "IsDeliveryReceiptRequested": true,
  "IsReadReceiptRequested": true,
  "IsDraft": true,
  "IsRead": true,
  "WebLink": "WebLink-value",
  "ChangeKey": "ChangeKey-value",
  "Categories": [
    "Categories-value"
  ],
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "message"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1546
{
  "Subject": "Subject-value",
  "Body": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "BodyPreview": "BodyPreview-value",
  "Importance": "Importance-value",
  "HasAttachments": true,
  "ParentFolderId": "ParentFolderId-value",
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
  "UniqueBody": {
    "ContentType": "ContentType-value",
    "Content": "Content-value"
  },
  "DateTimeReceived": "datetime-value",
  "DateTimeSent": "datetime-value",
  "IsDeliveryReceiptRequested": true,
  "IsReadReceiptRequested": true,
  "IsDraft": true,
  "IsRead": true,
  "WebLink": "WebLink-value",
  "ChangeKey": "ChangeKey-value",
  "Categories": [
    "Categories-value"
  ],
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```

<!-- uuid: 4e83cf34-3fd7-4259-8f33-171b33bbed3d
2015-10-15 03:41:19 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of message object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->