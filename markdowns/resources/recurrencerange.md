# RecurrenceRange resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|EndDate|Date||
|NumberOfOccurrences|Int32||
|RecurrenceTimeZone|String||
|StartDate|Date||
|Type|String| Possible values are: `EndDate`, `NoEnd`, `Numbered`.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.RecurrenceRange"
}-->

```json
{
  "EndDate": "String (timestamp)",
  "NumberOfOccurrences": 1024,
  "RecurrenceTimeZone": "String",
  "StartDate": "String (timestamp)",
  "Type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RecurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->