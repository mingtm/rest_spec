# Drive resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Drive](../api/drive_get.md) | [Drive](drive.md) |Read properties and relationships of drive object.|
|[Create Extension](../api/drive_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/drive_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create File](../api/drive_post_files.md) |[File](file.md)| Create a new File by posting to the Files collection.|
|[List Files](../api/drive_list_files.md) |[File](file.md) collection| Get a File object collection.|
|[Update](../api/drive_update.md) | [Drive](drive.md)	|Update Drive object. |
|[Delete](../api/drive_delete.md) | None |Delete Drive object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|EntityACL|[AccessControlList](accesscontrollist.md)||
|Id|String| Read-only.|

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|Files|[File](file.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Drive"
}-->

```json
{
  "EntityACL": {"@odata.type": "microsoft.graph.AccessControlList"},
  "Id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->