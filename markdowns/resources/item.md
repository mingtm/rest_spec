# Item resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Item](../api/item_get.md) | [Item](item.md) |Read properties and relationships of item object.|
|[Update](../api/item_update.md) | [Item](item.md)	|Update Item object. |
|[Delete](../api/item_delete.md) | None |Delete Item object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Categories|String collection||
|ChangeKey|String||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Id|String| Read-only.|
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Item"
}-->

```json
{
  "Categories": ["String"],
  "ChangeKey": "String",
  "CreatedDateTime": "String (timestamp)",
  "Id": "String (identifier)",
  "LastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->