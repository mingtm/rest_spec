# EventMessageRequest resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get EventMessageRequest](../api/eventmessagerequest_get.md) | [EventMessageRequest](eventmessagerequest.md) |Read properties and relationships of eventMessageRequest object.|
|[Create Attachment](../api/eventmessagerequest_post_attachments.md) |[Attachment](attachment.md)| Create a new Attachment by posting to the Attachments collection.|
|[List Attachments](../api/eventmessagerequest_list_attachments.md) |[Attachment](attachment.md) collection| Get a Attachment object collection.|
|[Create Extension](../api/eventmessagerequest_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/eventmessagerequest_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/eventmessagerequest_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/eventmessagerequest_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/eventmessagerequest_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/eventmessagerequest_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/eventmessagerequest_update.md) | [EventMessageRequest](eventmessagerequest.md)	|Update EventMessageRequest object. |
|[Delete](../api/eventmessagerequest_delete.md) | None |Delete EventMessageRequest object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|BccRecipients|[Recipient](recipient.md) collection||
|Body|[ItemBody](itembody.md)||
|BodyPreview|String||
|Categories|String collection||
|CcRecipients|[Recipient](recipient.md) collection||
|ChangeKey|String||
|ConversationId|String||
|ConversationIndex|Binary||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|EndDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|Flag|[FollowupFlag](followupflag.md)||
|From|[Recipient](recipient.md)||
|HasAttachments|Boolean||
|Id|String| Read-only.|
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|InferenceClassification|string| Possible values are: `Focused`, `Other`.|
|InternetMessageId|String||
|IsAllDay|Boolean||
|IsDeliveryReceiptRequested|Boolean||
|IsDraft|Boolean||
|IsOutOfDate|Boolean||
|IsRead|Boolean||
|IsReadReceiptRequested|Boolean||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Location|[Location](location.md)||
|MeetingMessageType|string| Possible values are: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTentativelyAccepted`, `MeetingDeclined`.|
|ParentFolderId|String||
|PreviousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|PreviousLocation|[Location](location.md)||
|PreviousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|ReceivedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Recurrence|[PatternedRecurrence](patternedrecurrence.md)||
|ReplyTo|[Recipient](recipient.md) collection||
|ResponseRequested|Boolean||
|Sender|[Recipient](recipient.md)||
|SentDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|StartDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|Subject|String||
|ToRecipients|[Recipient](recipient.md) collection||
|Type|string| Possible values are: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|UniqueBody|[ItemBody](itembody.md)||
|UnsubscribeData|String collection||
|UnsubscribeEnabled|Boolean||
|WebLink|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Attachments|[Attachment](attachment.md) collection| Read-only. Nullable.|
|Event|[Event](event.md)| Read-only. Nullable.|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.EventMessageRequest"
}-->

```json
{
  "BccRecipients": [{"@odata.type": "microsoft.graph.Recipient"}],
  "Body": {"@odata.type": "microsoft.graph.ItemBody"},
  "BodyPreview": "String",
  "Categories": ["String"],
  "CcRecipients": [{"@odata.type": "microsoft.graph.Recipient"}],
  "ChangeKey": "String",
  "ConversationId": "String",
  "ConversationIndex": "Binary",
  "CreatedDateTime": "String (timestamp)",
  "EndDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Flag": {"@odata.type": "microsoft.graph.FollowupFlag"},
  "From": {"@odata.type": "microsoft.graph.Recipient"},
  "HasAttachments": true,
  "Id": "String (identifier)",
  "Importance": "string",
  "InferenceClassification": "string",
  "InternetMessageId": "String",
  "IsAllDay": true,
  "IsDeliveryReceiptRequested": true,
  "IsDraft": true,
  "IsOutOfDate": true,
  "IsRead": true,
  "IsReadReceiptRequested": true,
  "LastModifiedDateTime": "String (timestamp)",
  "Location": {"@odata.type": "microsoft.graph.Location"},
  "MeetingMessageType": "string",
  "ParentFolderId": "String",
  "PreviousEndDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "PreviousLocation": {"@odata.type": "microsoft.graph.Location"},
  "PreviousStartDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "ReceivedDateTime": "String (timestamp)",
  "Recurrence": {"@odata.type": "microsoft.graph.PatternedRecurrence"},
  "ReplyTo": [{"@odata.type": "microsoft.graph.Recipient"}],
  "ResponseRequested": true,
  "Sender": {"@odata.type": "microsoft.graph.Recipient"},
  "SentDateTime": "String (timestamp)",
  "StartDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Subject": "String",
  "ToRecipients": [{"@odata.type": "microsoft.graph.Recipient"}],
  "Type": "string",
  "UniqueBody": {"@odata.type": "microsoft.graph.ItemBody"},
  "UnsubscribeData": ["String"],
  "UnsubscribeEnabled": true,
  "WebLink": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "EventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->