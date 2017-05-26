# Reminder resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChangeKey|String||
|EventEndTime|[DateTimeTimeZone](datetimetimezone.md)||
|EventId|String||
|EventLocation|[Location](location.md)||
|EventStartTime|[DateTimeTimeZone](datetimetimezone.md)||
|EventSubject|String||
|EventWebLink|String||
|ReminderFireTime|[DateTimeTimeZone](datetimetimezone.md)||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Reminder"
}-->

```json
{
  "ChangeKey": "String",
  "EventEndTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "EventId": "String",
  "EventLocation": {"@odata.type": "microsoft.graph.Location"},
  "EventStartTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "EventSubject": "String",
  "EventWebLink": "String",
  "ReminderFireTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->