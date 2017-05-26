# MeetingTimeCandidatesResult resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|EmptySuggestionsHint|String||
|MeetingTimeSlots|[MeetingTimeCandidate](meetingtimecandidate.md) collection||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.MeetingTimeCandidatesResult"
}-->

```json
{
  "EmptySuggestionsHint": "String",
  "MeetingTimeSlots": [{"@odata.type": "microsoft.graph.MeetingTimeCandidate"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MeetingTimeCandidatesResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->