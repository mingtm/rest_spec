# Location resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Address|[PhysicalAddress](physicaladdress.md)||
|Coordinates|[GeoCoordinates](geocoordinates.md)||
|DisplayName|String||
|LocationEmailAddress|String||
|LocationUri|String||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Location"
}-->

```json
{
  "Address": {"@odata.type": "microsoft.graph.PhysicalAddress"},
  "Coordinates": {"@odata.type": "microsoft.graph.GeoCoordinates"},
  "DisplayName": "String",
  "LocationEmailAddress": "String",
  "LocationUri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->