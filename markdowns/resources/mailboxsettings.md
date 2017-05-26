# MailboxSettings resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AutomaticRepliesSetting|[AutomaticRepliesSetting](automaticrepliessetting.md)||
|Language|[LocaleInfo](localeinfo.md)||
|TimeZone|String||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.MailboxSettings"
}-->

```json
{
  "AutomaticRepliesSetting": {"@odata.type": "microsoft.graph.AutomaticRepliesSetting"},
  "Language": {"@odata.type": "microsoft.graph.LocaleInfo"},
  "TimeZone": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->