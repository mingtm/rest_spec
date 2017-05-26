# TimeConstraint resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ActivityDomain|String| Possible values are: `Unknown`, `Work`, `Personal`.|
|Timeslots|[TimeSlot](timeslot.md) collection||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.TimeConstraint"
}-->

```json
{
  "ActivityDomain": "String",
  "Timeslots": [{"@odata.type": "microsoft.graph.TimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TimeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->