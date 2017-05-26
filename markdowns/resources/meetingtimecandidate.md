# MeetingTimeCandidate resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AttendeeAvailability|[AttendeeAvailability](attendeeavailability.md) collection||
|Confidence|Double||
|Locations|[Location](location.md) collection||
|MeetingTimeSlot|[TimeSlot](timeslot.md)||
|OrganizerAvailability|String| Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|SuggestionHint|String||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.MeetingTimeCandidate"
}-->

```json
{
  "AttendeeAvailability": [{"@odata.type": "microsoft.graph.AttendeeAvailability"}],
  "Confidence": 1024,
  "Locations": [{"@odata.type": "microsoft.graph.Location"}],
  "MeetingTimeSlot": {"@odata.type": "microsoft.graph.TimeSlot"},
  "OrganizerAvailability": "String",
  "SuggestionHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MeetingTimeCandidate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->