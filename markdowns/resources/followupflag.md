# FollowupFlag resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|CompletedDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|DueDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|FlagStatus|String| Possible values are: `NotFlagged`, `Complete`, `Flagged`.|
|StartDateTime|[DateTimeTimeZone](datetimetimezone.md)||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.FollowupFlag"
}-->

```json
{
  "CompletedDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "DueDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "FlagStatus": "String",
  "StartDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FollowupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->