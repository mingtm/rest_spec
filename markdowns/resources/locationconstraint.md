# LocationConstraint resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|IsRequired|Boolean||
|Locations|[LocationConstraintItem](locationconstraintitem.md) collection||
|SuggestLocation|Boolean||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.LocationConstraint"
}-->

```json
{
  "IsRequired": true,
  "Locations": [{"@odata.type": "microsoft.graph.LocationConstraintItem"}],
  "SuggestLocation": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "LocationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->