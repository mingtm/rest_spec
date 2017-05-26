# Post resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Post](../api/post_get.md) | [Post](post.md) |Read properties and relationships of post object.|
|[Create Attachment](../api/post_post_attachments.md) |[Attachment](attachment.md)| Create a new Attachment by posting to the Attachments collection.|
|[List Attachments](../api/post_list_attachments.md) |[Attachment](attachment.md) collection| Get a Attachment object collection.|
|[Create Extension](../api/post_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/post_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/post_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/post_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/post_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/post_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/post_update.md) | [Post](post.md)	|Update Post object. |
|[Delete](../api/post_delete.md) | None |Delete Post object. |
|[Forward](../api/post_forward.md)|None||
|[Reply](../api/post_reply.md)|None||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Body|[ItemBody](itembody.md)||
|Categories|String collection||
|ChangeKey|String||
|ConversationId|String||
|ConversationThreadId|String||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|From|[Recipient](recipient.md)||
|HasAttachments|Boolean||
|Id|String| Read-only.|
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|NewParticipants|[Recipient](recipient.md) collection||
|ReceivedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Sender|[Recipient](recipient.md)||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Attachments|[Attachment](attachment.md) collection| Read-only. Nullable.|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|InReplyTo|[Post](post.md)| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Post"
}-->

```json
{
  "Body": {"@odata.type": "microsoft.graph.ItemBody"},
  "Categories": ["String"],
  "ChangeKey": "String",
  "ConversationId": "String",
  "ConversationThreadId": "String",
  "CreatedDateTime": "String (timestamp)",
  "From": {"@odata.type": "microsoft.graph.Recipient"},
  "HasAttachments": true,
  "Id": "String (identifier)",
  "LastModifiedDateTime": "String (timestamp)",
  "NewParticipants": [{"@odata.type": "microsoft.graph.Recipient"}],
  "ReceivedDateTime": "String (timestamp)",
  "Sender": {"@odata.type": "microsoft.graph.Recipient"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->