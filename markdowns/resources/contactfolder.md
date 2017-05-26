# ContactFolder resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get ContactFolder](../api/contactfolder_get.md) | [ContactFolder](contactfolder.md) |Read properties and relationships of contactFolder object.|
|[Create ContactFolder](../api/contactfolder_post_childfolders.md) |[ContactFolder](contactfolder.md)| Create a new ContactFolder by posting to the ChildFolders collection.|
|[List ChildFolders](../api/contactfolder_list_childfolders.md) |[ContactFolder](contactfolder.md) collection| Get a ContactFolder object collection.|
|[Create Contact](../api/contactfolder_post_contacts.md) |[Contact](contact.md)| Create a new Contact by posting to the Contacts collection.|
|[List Contacts](../api/contactfolder_list_contacts.md) |[Contact](contact.md) collection| Get a Contact object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/contactfolder_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/contactfolder_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/contactfolder_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/contactfolder_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/contactfolder_update.md) | [ContactFolder](contactfolder.md)	|Update ContactFolder object. |
|[Delete](../api/contactfolder_delete.md) | None |Delete ContactFolder object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|DisplayName|String||
|Id|String| Read-only.|
|ParentFolderId|String||
|WellKnownName|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolders|[ContactFolder](contactfolder.md) collection| Read-only. Nullable.|
|Contacts|[Contact](contact.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ContactFolder"
}-->

```json
{
  "DisplayName": "String",
  "Id": "String (identifier)",
  "ParentFolderId": "String",
  "WellKnownName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ContactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->