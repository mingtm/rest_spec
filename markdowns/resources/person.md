# Person resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Person](../api/person_get.md) | [Person](person.md) |Read properties and relationships of person object.|
|[Update](../api/person_update.md) | [Person](person.md)	|Update Person object. |
|[Delete](../api/person_delete.md) | None |Delete Person object. |

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Birthday|String||
|CompanyName|String||
|Department|String||
|DisplayName|String||
|EmailAddresses|[RankedEmailAddress](rankedemailaddress.md) collection||
|GivenName|String||
|Id|String| Read-only.|
|IsFavorite|Boolean||
|MailboxType|String||
|OfficeLocation|String||
|PersonNotes|String||
|PersonType|String||
|Phones|[Phone](phone.md) collection||
|PostalAddresses|[Location](location.md) collection||
|Profession|String||
|Sources|[PersonDataSource](persondatasource.md) collection||
|Surname|String||
|Title|String||
|Websites|[Website](website.md) collection||
|YomiCompany|String||

### Relationships
None


### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Person"
}-->

```json
{
  "Birthday": "String",
  "CompanyName": "String",
  "Department": "String",
  "DisplayName": "String",
  "EmailAddresses": [{"@odata.type": "microsoft.graph.RankedEmailAddress"}],
  "GivenName": "String",
  "Id": "String (identifier)",
  "IsFavorite": true,
  "MailboxType": "String",
  "OfficeLocation": "String",
  "PersonNotes": "String",
  "PersonType": "String",
  "Phones": [{"@odata.type": "microsoft.graph.Phone"}],
  "PostalAddresses": [{"@odata.type": "microsoft.graph.Location"}],
  "Profession": "String",
  "Sources": [{"@odata.type": "microsoft.graph.PersonDataSource"}],
  "Surname": "String",
  "Title": "String",
  "Websites": [{"@odata.type": "microsoft.graph.Website"}],
  "YomiCompany": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->