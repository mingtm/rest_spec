# Notification resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Notification](../api/notification_get.md) | [Notification](notification.md) |Read properties and relationships of notification object.|
|[Update](../api/notification_update.md) | [Notification](notification.md)	|Update Notification object. |
|[Delete](../api/notification_delete.md) | None |Delete Notification object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeType|string| Possible values are: `Created`, `Updated`, `Deleted`, `Acknowledgment`, `Missed`.|
|Id|String| Read-only.|
|Resource|String||
|ResourceCount|Int32||
|SequenceNumber|Int32||
|SubscriptionExpirationDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|SubscriptionId|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|ResourceData|[Entity](entity.md)| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Notification"
}-->

```json
{
  "ChangeType": "string",
  "Id": "String (identifier)",
  "Resource": "String",
  "ResourceCount": 1024,
  "SequenceNumber": 1024,
  "SubscriptionExpirationDateTime": "String (timestamp)",
  "SubscriptionId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->