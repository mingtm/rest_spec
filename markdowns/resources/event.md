# Event resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Event](../api/event_get.md) | [Event](event.md) |Read properties and relationships of event object.|
|[Create Attachment](../api/event_post_attachments.md) |[Attachment](attachment.md)| Create a new Attachment by posting to the Attachments collection.|
|[List Attachments](../api/event_list_attachments.md) |[Attachment](attachment.md) collection| Get a Attachment object collection.|
|[Create Extension](../api/event_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/event_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create Event](../api/event_post_instances.md) |[Event](event.md)| Create a new Event by posting to the Instances collection.|
|[List Instances](../api/event_list_instances.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/event_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/event_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/event_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/event_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/event_update.md) | [Event](event.md)	|Update Event object. |
|[Delete](../api/event_delete.md) | None |Delete Event object. |
|[Accept](../api/event_accept.md)|None||
|[Cancel](../api/event_cancel.md)|None||
|[Checkin](../api/event_checkin.md)|None||
|[Decline](../api/event_decline.md)|None||
|[Dismissreminder](../api/event_dismissreminder.md)|None||
|[Snoozereminder](../api/event_snoozereminder.md)|None||
|[Tentativelyaccept](../api/event_tentativelyaccept.md)|None||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Attendance|[AttendanceInfo](attendanceinfo.md) collection||
|Attendees|[Attendee](attendee.md) collection||
|Body|[ItemBody](itembody.md)||
|BodyPreview|String||
|Categories|String collection||
|ChangeKey|String||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|End|[DateTimeTimeZone](datetimetimezone.md)||
|HasAttachments|Boolean||
|Id|String| Read-only.|
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|IsAllDay|Boolean||
|IsCancelled|Boolean||
|IsOrganizer|Boolean||
|IsReminderOn|Boolean||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Location|[Location](location.md)||
|OnlineMeetingUrl|String||
|Organizer|[Recipient](recipient.md)||
|OriginalEndTimeZone|String||
|OriginalStart|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|OriginalStartTimeZone|String||
|Recurrence|[PatternedRecurrence](patternedrecurrence.md)||
|ReminderMinutesBeforeStart|Int32||
|ResponseRequested|Boolean||
|ResponseStatus|[ResponseStatus](responsestatus.md)||
|Sensitivity|string| Possible values are: `Normal`, `Personal`, `Private`, `Confidential`.|
|SeriesMasterId|String||
|ShowAs|string| Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|Start|[DateTimeTimeZone](datetimetimezone.md)||
|Subject|String||
|Type|string| Possible values are: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|WebLink|String||
|iCalUId|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Attachments|[Attachment](attachment.md) collection| Read-only. Nullable.|
|Calendar|[Calendar](calendar.md)| Read-only. Nullable.|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|Instances|[Event](event.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Event"
}-->

```json
{
  "Attendance": [{"@odata.type": "microsoft.graph.AttendanceInfo"}],
  "Attendees": [{"@odata.type": "microsoft.graph.Attendee"}],
  "Body": {"@odata.type": "microsoft.graph.ItemBody"},
  "BodyPreview": "String",
  "Categories": ["String"],
  "ChangeKey": "String",
  "CreatedDateTime": "String (timestamp)",
  "End": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "HasAttachments": true,
  "Id": "String (identifier)",
  "Importance": "string",
  "IsAllDay": true,
  "IsCancelled": true,
  "IsOrganizer": true,
  "IsReminderOn": true,
  "LastModifiedDateTime": "String (timestamp)",
  "Location": {"@odata.type": "microsoft.graph.Location"},
  "OnlineMeetingUrl": "String",
  "Organizer": {"@odata.type": "microsoft.graph.Recipient"},
  "OriginalEndTimeZone": "String",
  "OriginalStart": "String (timestamp)",
  "OriginalStartTimeZone": "String",
  "Recurrence": {"@odata.type": "microsoft.graph.PatternedRecurrence"},
  "ReminderMinutesBeforeStart": 1024,
  "ResponseRequested": true,
  "ResponseStatus": {"@odata.type": "microsoft.graph.ResponseStatus"},
  "Sensitivity": "string",
  "SeriesMasterId": "String",
  "ShowAs": "string",
  "Start": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Subject": "String",
  "Type": "string",
  "WebLink": "String",
  "iCalUId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->