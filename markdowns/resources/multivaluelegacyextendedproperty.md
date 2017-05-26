# MultiValueLegacyExtendedProperty resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get MultiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty_get.md) | [MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) |Read properties and relationships of multiValueLegacyExtendedProperty object.|
|[Update](../api/multivaluelegacyextendedproperty_update.md) | [MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)	|Update MultiValueLegacyExtendedProperty object. |
|[Delete](../api/multivaluelegacyextendedproperty_delete.md) | None |Delete MultiValueLegacyExtendedProperty object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|PropertyId|String| Read-only.|
|Value|String collection||

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.MultiValueLegacyExtendedProperty"
}-->

```json
{
  "PropertyId": "String (identifier)",
  "Value": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MultiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->