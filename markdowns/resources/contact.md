# Contact resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Contact](../api/contact_get.md) | [Contact](contact.md) |Read properties and relationships of contact object.|
|[Create Extension](../api/contact_post_extensions.md) |[Extension](extension.md)| Create a new Extension by posting to the Extensions collection.|
|[List Extensions](../api/contact_list_extensions.md) |[Extension](extension.md) collection| Get a Extension object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/contact_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/contact_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/contact_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/contact_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Update](../api/contact_update.md) | [Contact](contact.md)	|Update Contact object. |
|[Delete](../api/contact_delete.md) | None |Delete Contact object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AssistantName|String||
|Birthday|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Categories|String collection||
|ChangeKey|String||
|Children|String collection||
|CompanyName|String||
|CreatedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Department|String||
|DisplayName|String||
|EmailAddresses|[EmailAddress](emailaddress.md) collection||
|FileAs|String||
|Flag|[FollowupFlag](followupflag.md)||
|Gender|String||
|Generation|String||
|GivenName|String||
|Id|String| Read-only.|
|ImAddresses|String collection||
|Initials|String||
|JobTitle|String||
|LastModifiedDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|Manager|String||
|MiddleName|String||
|NickName|String||
|OfficeLocation|String||
|ParentFolderId|String||
|PersonalNotes|String||
|Phones|[Phone](phone.md) collection||
|PostalAddresses|[PhysicalAddress](physicaladdress.md) collection||
|Profession|String||
|SpouseName|String||
|Surname|String||
|Title|String||
|Websites|[Website](website.md) collection||
|WeddingAnniversary|Date||
|YomiCompanyName|String||
|YomiGivenName|String||
|YomiSurname|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Extensions|[Extension](extension.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|Photo|[Photo](photo.md)| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contact"
}-->

```json
{
  "AssistantName": "String",
  "Birthday": "String (timestamp)",
  "Categories": ["String"],
  "ChangeKey": "String",
  "Children": ["String"],
  "CompanyName": "String",
  "CreatedDateTime": "String (timestamp)",
  "Department": "String",
  "DisplayName": "String",
  "EmailAddresses": [{"@odata.type": "microsoft.graph.EmailAddress"}],
  "FileAs": "String",
  "Flag": {"@odata.type": "microsoft.graph.FollowupFlag"},
  "Gender": "String",
  "Generation": "String",
  "GivenName": "String",
  "Id": "String (identifier)",
  "ImAddresses": ["String"],
  "Initials": "String",
  "JobTitle": "String",
  "LastModifiedDateTime": "String (timestamp)",
  "Manager": "String",
  "MiddleName": "String",
  "NickName": "String",
  "OfficeLocation": "String",
  "ParentFolderId": "String",
  "PersonalNotes": "String",
  "Phones": [{"@odata.type": "microsoft.graph.Phone"}],
  "PostalAddresses": [{"@odata.type": "microsoft.graph.PhysicalAddress"}],
  "Profession": "String",
  "SpouseName": "String",
  "Surname": "String",
  "Title": "String",
  "Websites": [{"@odata.type": "microsoft.graph.Website"}],
  "WeddingAnniversary": "String (timestamp)",
  "YomiCompanyName": "String",
  "YomiGivenName": "String",
  "YomiSurname": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->