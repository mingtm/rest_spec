# AccessControlEntry resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AccessRight|String| Possible values are: `Read`, `Write`.|
|AccessType|String| Possible values are: `Deny`, `Grant`.|
|Claim|[Claim](claim.md)||

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.AccessControlEntry"
}-->

```json
{
  "AccessRight": "String",
  "AccessType": "String",
  "Claim": {"@odata.type": "microsoft.graph.Claim"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "AccessControlEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->