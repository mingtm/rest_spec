# ReferenceAttachment resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get ReferenceAttachment](../api/referenceattachment_get.md) | [ReferenceAttachment](referenceattachment.md) |Read properties and relationships of referenceAttachment object.|
|[Update](../api/referenceattachment_update.md) | [ReferenceAttachment](referenceattachment.md)	|Update ReferenceAttachment object. |
|[Delete](../api/referenceattachment_delete.md) | None |Delete ReferenceAttachment object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ContentType|String||
|Id|String| Read-only.|
|IsFolder|Boolean||
|IsInline|Boolean||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Name|String||
|Permission|string| Possible values are: `Other`, `View`, `Edit`.|
|PreviewUrl|String||
|ProviderType|string| Possible values are: `Other`, `OneDriveBusiness`, `OneDriveConsumer`, `Dropbox`.|
|Size|Int32||
|SourceUrl|String||
|ThumbnailUrl|String||

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ReferenceAttachment"
}-->

```json
{
  "ContentType": "String",
  "Id": "String (identifier)",
  "IsFolder": true,
  "IsInline": true,
  "LastModifiedDateTime": "String (timestamp)",
  "Name": "String",
  "Permission": "string",
  "PreviewUrl": "String",
  "ProviderType": "string",
  "Size": 1024,
  "SourceUrl": "String",
  "ThumbnailUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ReferenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->