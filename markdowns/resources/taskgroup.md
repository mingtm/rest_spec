# TaskGroup resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get TaskGroup](../api/taskgroup_get.md) | [TaskGroup](taskgroup.md) |Read properties and relationships of taskGroup object.|
|[Create TaskFolder](../api/taskgroup_post_taskfolders.md) |[TaskFolder](taskfolder.md)| Create a new TaskFolder by posting to the TaskFolders collection.|
|[List TaskFolders](../api/taskgroup_list_taskfolders.md) |[TaskFolder](taskfolder.md) collection| Get a TaskFolder object collection.|
|[Update](../api/taskgroup_update.md) | [TaskGroup](taskgroup.md)	|Update TaskGroup object. |
|[Delete](../api/taskgroup_delete.md) | None |Delete TaskGroup object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeKey|String||
|GroupKey|Guid||
|Id|String| Read-only.|
|IsDefaultGroup|Boolean||
|Name|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|TaskFolders|[TaskFolder](taskfolder.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.TaskGroup"
}-->

```json
{
  "ChangeKey": "String",
  "GroupKey": "Guid",
  "Id": "String (identifier)",
  "IsDefaultGroup": true,
  "Name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->