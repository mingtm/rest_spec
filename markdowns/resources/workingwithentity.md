# WorkingWithEntity resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get WorkingWithEntity](../api/workingwithentity_get.md) | [WorkingWithEntity](workingwithentity.md) |Read properties and relationships of workingWithEntity object.|
|[Create Extension](../api/workingwithentity_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/workingwithentity_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Update](../api/workingwithentity_update.md) | [WorkingWithEntity](workingwithentity.md)	|Update WorkingWithEntity object. |
|[Delete](../api/workingwithentity_delete.md) | None |Delete WorkingWithEntity object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Email|String||
|EntityACL|[AccessControlList](accesscontrollist.md)||
|Id|String| Read-only.|
|PreferredName|String||

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
  "@odata.type": "microsoft.graph.WorkingWithEntity"
}-->

```json
{
  "Email": "String",
  "EntityACL": {"@odata.type": "microsoft.graph.AccessControlList"},
  "Id": "String (identifier)",
  "PreferredName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorkingWithEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->