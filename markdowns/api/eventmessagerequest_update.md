# Update eventmessagerequest

Update the properties of eventmessagerequest object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http

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
|EndDateTime|DateTimeTimeZone||
|Flag|FollowupFlag||
|From|Recipient||
|HasAttachments|Boolean||
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|InferenceClassification|string| Possible values are: `Focused`, `Other`.|
|InternetMessageId|String||
|IsAllDay|Boolean||
|IsDeliveryReceiptRequested|Boolean||
|IsDraft|Boolean||
|IsOutOfDate|Boolean||
|IsRead|Boolean||
|IsReadReceiptRequested|Boolean||
|LastModifiedDateTime|DateTimeOffset||
|Location|Location||
|MeetingMessageType|string| Possible values are: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTentativelyAccepted`, `MeetingDeclined`.|
|ParentFolderId|String||
|PreviousEndDateTime|DateTimeTimeZone||
|PreviousLocation|Location||
|PreviousStartDateTime|DateTimeTimeZone||
|ReceivedDateTime|DateTimeOffset||
|Recurrence|PatternedRecurrence||
|ReplyTo|Recipient||
|ResponseRequested|Boolean||
|Sender|Recipient||
|SentDateTime|DateTimeOffset||
|StartDateTime|DateTimeTimeZone||
|Subject|String||
|ToRecipients|Recipient||
|Type|string| Possible values are: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|UniqueBody|ItemBody||
|UnsubscribeData|String||
|UnsubscribeEnabled|Boolean||
|WebLink|String||

### Response
If successful, this method returns a `200 OK` response code and updated [EventMessageRequest](../resources/eventmessagerequest.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_eventmessagerequest"
}-->
```http

Content-type: application/json
Content-length: 938

{
  "PreviousLocation": {
    "DisplayName": "DisplayName-value",
    "LocationEmailAddress": "LocationEmailAddress-value",
    "Address": {
      "Type": "Type-value",
      "PostOfficeBox": "PostOfficeBox-value",
      "Street": "Street-value",
      "City": "City-value",
      "State": "State-value",
      "CountryOrRegion": "CountryOrRegion-value",
      "PostalCode": "PostalCode-value"
    },
    "Coordinates": {
      "Altitude": 99,
      "Latitude": 99,
      "Longitude": 99,
      "Accuracy": 99,
      "AltitudeAccuracy": 99
    },
    "LocationUri": "LocationUri-value"
  },
  "PreviousStartDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  },
  "PreviousEndDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  },
  "ResponseRequested": true,
  "MeetingMessageType": "MeetingMessageType-value",
  "StartDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  }
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.EventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 938

{
  "PreviousLocation": {
    "DisplayName": "DisplayName-value",
    "LocationEmailAddress": "LocationEmailAddress-value",
    "Address": {
      "Type": "Type-value",
      "PostOfficeBox": "PostOfficeBox-value",
      "Street": "Street-value",
      "City": "City-value",
      "State": "State-value",
      "CountryOrRegion": "CountryOrRegion-value",
      "PostalCode": "PostalCode-value"
    },
    "Coordinates": {
      "Altitude": 99,
      "Latitude": 99,
      "Longitude": 99,
      "Accuracy": 99,
      "AltitudeAccuracy": 99
    },
    "LocationUri": "LocationUri-value"
  },
  "PreviousStartDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  },
  "PreviousEndDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  },
  "ResponseRequested": true,
  "MeetingMessageType": "MeetingMessageType-value",
  "StartDateTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessagerequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->