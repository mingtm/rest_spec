# Message resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Message](../api/message_get.md) | [Message](message.md) |Read properties and relationships of message object.|
|[Create Attachment](../api/message_post_attachments.md) |[Attachment](attachment.md)| Create a new Attachment by posting to the Attachments collection.|
|[List Attachments](../api/message_list_attachments.md) |[Attachment](attachment.md) collection| Get a Attachment object collection.|
|[Create Extension](../api/message_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/message_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/message_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/message_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/message_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/message_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/message_update.md) | [Message](message.md)	|Update Message object. |
|[Delete](../api/message_delete.md) | None |Delete Message object. |
|[Copy](../api/message_copy.md)|[Message](message.md)||
|[Createforward](../api/message_createforward.md)|[Message](message.md)||
|[Createreply](../api/message_createreply.md)|[Message](message.md)||
|[Createreplyall](../api/message_createreplyall.md)|[Message](message.md)||
|[Forward](../api/message_forward.md)|None||
|[Move](../api/message_move.md)|[Message](message.md)||
|[Reply](../api/message_reply.md)|None||
|[Replyall](../api/message_replyall.md)|None||
|[Send](../api/message_send.md)|None||
|[Unsubscribe](../api/message_unsubscribe.md)|None||

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
|Flag|[FollowupFlag](followupflag.md)||
|From|[Recipient](recipient.md)||
|HasAttachments|Boolean||
|Id|String| Read-only.|
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|InferenceClassification|string| Possible values are: `Focused`, `Other`.|
|InternetMessageId|String||
|IsDeliveryReceiptRequested|Boolean||
|IsDraft|Boolean||
|IsRead|Boolean||
|IsReadReceiptRequested|Boolean||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|ParentFolderId|String||
|ReceivedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|ReplyTo|[Recipient](recipient.md) collection||
|Sender|[Recipient](recipient.md)||
|SentDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Subject|String||
|ToRecipients|[Recipient](recipient.md) collection||
|UniqueBody|[ItemBody](itembody.md)||
|UnsubscribeData|String collection||
|UnsubscribeEnabled|Boolean||
|WebLink|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Attachments|[Attachment](attachment.md) collection| Read-only. Nullable.|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Message"
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
  "Flag": {"@odata.type": "microsoft.graph.FollowupFlag"},
  "From": {"@odata.type": "microsoft.graph.Recipient"},
  "HasAttachments": true,
  "Id": "String (identifier)",
  "Importance": "string",
  "InferenceClassification": "string",
  "InternetMessageId": "String",
  "IsDeliveryReceiptRequested": true,
  "IsDraft": true,
  "IsRead": true,
  "IsReadReceiptRequested": true,
  "LastModifiedDateTime": "String (timestamp)",
  "ParentFolderId": "String",
  "ReceivedDateTime": "String (timestamp)",
  "ReplyTo": [{"@odata.type": "microsoft.graph.Recipient"}],
  "Sender": {"@odata.type": "microsoft.graph.Recipient"},
  "SentDateTime": "String (timestamp)",
  "Subject": "String",
  "ToRecipients": [{"@odata.type": "microsoft.graph.Recipient"}],
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
  "description": "Message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->