# TaskFolder resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get TaskFolder](../api/taskfolder_get.md) | [TaskFolder](taskfolder.md) |Read properties and relationships of taskFolder object.|
|[Create Task](../api/taskfolder_post_tasks.md) |[Task](task.md)| Create a new Task by posting to the Tasks collection.|
|[List Tasks](../api/taskfolder_list_tasks.md) |[Task](task.md) collection| Get a Task object collection.|
|[Update](../api/taskfolder_update.md) | [TaskFolder](taskfolder.md)	|Update TaskFolder object. |
|[Delete](../api/taskfolder_delete.md) | None |Delete TaskFolder object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeKey|String||
|Id|String| Read-only.|
|IsDefaultFolder|Boolean||
|Name|String||
|ParentGroupKey|Guid||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Tasks|[Task](task.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.TaskFolder"
}-->

```json
{
  "ChangeKey": "String",
  "Id": "String (identifier)",
  "IsDefaultFolder": true,
  "Name": "String",
  "ParentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->