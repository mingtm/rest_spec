# AutomaticRepliesSetting resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ExternalAudience|String| Possible values are: `None`, `ContactsOnly`, `All`.|
|ExternalReplyMessage|String||
|InternalReplyMessage|String||
|ScheduledEndDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|ScheduledStartDateTime|[DateTimeTimeZone](datetimetimezone.md)||
|Status|String| Possible values are: `Disabled`, `AlwaysEnabled`, `Scheduled`.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.AutomaticRepliesSetting"
}-->

```json
{
  "ExternalAudience": "String",
  "ExternalReplyMessage": "String",
  "InternalReplyMessage": "String",
  "ScheduledEndDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "ScheduledStartDateTime": {"@odata.type": "microsoft.graph.DateTimeTimeZone"},
  "Status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "AutomaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->