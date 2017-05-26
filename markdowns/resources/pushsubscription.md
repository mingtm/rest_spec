# PushSubscription resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get PushSubscription](../api/pushsubscription_get.md) | [PushSubscription](pushsubscription.md) |Read properties and relationships of pushSubscription object.|
|[Update](../api/pushsubscription_update.md) | [PushSubscription](pushsubscription.md)	|Update PushSubscription object. |
|[Delete](../api/pushsubscription_delete.md) | None |Delete PushSubscription object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeType|string| Possible values are: `Created`, `Updated`, `Deleted`, `Acknowledgment`, `Missed`.|
|ClientState|String||
|Id|String| Read-only.|
|NotificationURL|String||
|Resource|String||
|SubscriptionExpirationDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.PushSubscription"
}-->

```json
{
  "ChangeType": "string",
  "ClientState": "String",
  "Id": "String (identifier)",
  "NotificationURL": "String",
  "Resource": "String",
  "SubscriptionExpirationDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "PushSubscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->