# AttendeeAvailability resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Attendee|[AttendeeBase](attendeebase.md)||
|Availability|String| Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.AttendeeAvailability"
}-->

```json
{
  "Attendee": {"@odata.type": "microsoft.graph.AttendeeBase"},
  "Availability": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "AttendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->