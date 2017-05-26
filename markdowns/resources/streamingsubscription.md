# StreamingSubscription resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get StreamingSubscription](../api/streamingsubscription_get.md) | [StreamingSubscription](streamingsubscription.md) |Read properties and relationships of streamingSubscription object.|
|[Update](../api/streamingsubscription_update.md) | [StreamingSubscription](streamingsubscription.md)	|Update StreamingSubscription object. |
|[Delete](../api/streamingsubscription_delete.md) | None |Delete StreamingSubscription object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeType|string| Possible values are: `Created`, `Updated`, `Deleted`, `Acknowledgment`, `Missed`.|
|Id|String| Read-only.|
|Resource|String||

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.StreamingSubscription"
}-->

```json
{
  "ChangeType": "string",
  "Id": "String (identifier)",
  "Resource": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "StreamingSubscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->