# Update message

Update the properties of message object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/Messages/<Id>
PATCH /Users/<Id>/Messages/<Id>
PATCH /me/MailFolders/<Id>/Messages/<Id>
```
### Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

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
|ConversationIndex|Binary||
|CreatedDateTime|DateTimeOffset||
|Flag|FollowupFlag||
|From|Recipient||
|HasAttachments|Boolean||
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|InferenceClassification|string| Possible values are: `Focused`, `Other`.|
|InternetMessageId|String||
|IsDeliveryReceiptRequested|Boolean||
|IsDraft|Boolean||
|IsRead|Boolean||
|IsReadReceiptRequested|Boolean||
|LastModifiedDateTime|DateTimeOffset||
|ParentFolderId|String||
|ReceivedDateTime|DateTimeOffset||
|ReplyTo|Recipient||
|Sender|Recipient||
|SentDateTime|DateTimeOffset||
|Subject|String||
|ToRecipients|Recipient||
|UniqueBody|ItemBody||
|UnsubscribeData|String||
|UnsubscribeEnabled|Boolean||
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
PATCH https://graph.microsoft.com/beta/me/Messages/<Id>
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
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->