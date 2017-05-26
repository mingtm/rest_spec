# Task resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Task](../api/task_get.md) | [Task](task.md) |Read properties and relationships of task object.|
|[Create MultiValueLegacyExtendedProperty](../api/task_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/task_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/task_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/task_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/task_update.md) | [Task](task.md)	|Update Task object. |
|[Delete](../api/task_delete.md) | None |Delete Task object. |
|[Complete](../api/task_complete.md)|[Task](task.md) collection||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AssignedTo|String||
|Body|[ItemBody](itembody.md)||
|Categories|String collection||
|ChangeKey|String||
|CompletedDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|DueDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|Id|String| Read-only.|
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|IsReminderOn|Boolean||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Owner|String||
|ParentFolderId|String||
|Recurrence|[PatternedRecurrence](patternedrecurrence.md)||
|ReminderDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|StartDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|Status|string| Possible values are: `NotStarted`, `InProgress`, `Completed`, `WaitingOnOthers`, `Deferred`.|
|Subject|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Task"
}-->

```json
{
  "AssignedTo": "String",
  "Body": {"@odata.type": "microsoft.graph.ItemBody"},
  "Categories": ["String"],
  "ChangeKey": "String",
  "CompletedDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "CreatedDateTime": "String (timestamp)",
  "DueDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Id": "String (identifier)",
  "Importance": "string",
  "IsReminderOn": true,
  "LastModifiedDateTime": "String (timestamp)",
  "Owner": "String",
  "ParentFolderId": "String",
  "Recurrence": {"@odata.type": "microsoft.graph.PatternedRecurrence"},
  "ReminderDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "StartDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Status": "string",
  "Subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Task resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->