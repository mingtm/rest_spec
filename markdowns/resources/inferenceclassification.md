# InferenceClassification resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get InferenceClassification](../api/inferenceclassification_get.md) | [InferenceClassification](inferenceclassification.md) |Read properties and relationships of inferenceClassification object.|
|[Create InferenceClassificationOverride](../api/inferenceclassification_post_overrides.md) |[InferenceClassificationOverride](inferenceclassificationoverride.md)| Create a new InferenceClassificationOverride by posting to the Overrides collection.|
|[List Overrides](../api/inferenceclassification_list_overrides.md) |[InferenceClassificationOverride](inferenceclassificationoverride.md) collection| Get a InferenceClassificationOverride object collection.|
|[Delete](../api/inferenceclassification_delete.md) | None |Delete InferenceClassification object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Id|String| Read-only.|

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Overrides|[InferenceClassificationOverride](inferenceclassificationoverride.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.InferenceClassification"
}-->

```json
{
  "Id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "InferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->