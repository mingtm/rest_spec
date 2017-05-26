# InferenceClassificationOverride resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get InferenceClassificationOverride](../api/inferenceclassificationoverride_get.md) | [InferenceClassificationOverride](inferenceclassificationoverride.md) |Read properties and relationships of inferenceClassificationOverride object.|
|[Update](../api/inferenceclassificationoverride_update.md) | [InferenceClassificationOverride](inferenceclassificationoverride.md)	|Update InferenceClassificationOverride object. |
|[Delete](../api/inferenceclassificationoverride_delete.md) | None |Delete InferenceClassificationOverride object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ClassifyAs|string| Possible values are: `Focused`, `Other`.|
|Id|String| Read-only.|
|SenderEmailAddress|[EmailAddress](emailaddress.md)||

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.InferenceClassificationOverride"
}-->

```json
{
  "ClassifyAs": "string",
  "Id": "String (identifier)",
  "SenderEmailAddress": {"@odata.type": "microsoft.graph.EmailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "InferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->