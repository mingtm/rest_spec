# File resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get File](../api/file_get.md) | [File](file.md) |Read properties and relationships of file object.|
|[Create Extension](../api/file_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/file_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Update](../api/file_update.md) | [File](file.md)	|Update File object. |
|[Delete](../api/file_delete.md) | None |Delete File object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|DateTimeCreated|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|DateTimeLastModified|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|EntityACL|[AccessControlList](accesscontrollist.md)||
|Id|String| Read-only.|
|Name|String||
|WebUrl|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.File"
}-->

```json
{
  "DateTimeCreated": "String (timestamp)",
  "DateTimeLastModified": "String (timestamp)",
  "EntityACL": {"@odata.type": "microsoft.graph.AccessControlList"},
  "Id": "String (identifier)",
  "Name": "String",
  "WebUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "File resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->