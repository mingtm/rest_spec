# MailFolder resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get MailFolder](../api/mailfolder_get.md) | [MailFolder](mailfolder.md) |Read properties and relationships of mailFolder object.|
|[Create MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| Create a new MailFolder by posting to the ChildFolders collection.|
|[List ChildFolders](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md) collection| Get a MailFolder object collection.|
|[Create Message](../api/mailfolder_post_messages.md) |[Message](message.md)| Create a new Message by posting to the Messages collection.|
|[List Messages](../api/mailfolder_list_messages.md) |[Message](message.md) collection| Get a Message object collection.|
|[Create MultiValueLegacyExtendedProperty](../api/mailfolder_post_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Create a new MultiValueLegacyExtendedProperty by posting to the MultiValueExtendedProperties collection.|
|[List MultiValueExtendedProperties](../api/mailfolder_list_multivalueextendedproperties.md) |[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Get a MultiValueLegacyExtendedProperty object collection.|
|[Create SingleValueLegacyExtendedProperty](../api/mailfolder_post_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Create a new SingleValueLegacyExtendedProperty by posting to the SingleValueExtendedProperties collection.|
|[List SingleValueExtendedProperties](../api/mailfolder_list_singlevalueextendedproperties.md) |[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Get a SingleValueLegacyExtendedProperty object collection.|
|[Create UserConfiguration](../api/mailfolder_post_userconfigurations.md) |[UserConfiguration](userconfiguration.md)| Create a new UserConfiguration by posting to the UserConfigurations collection.|
|[List UserConfigurations](../api/mailfolder_list_userconfigurations.md) |[UserConfiguration](userconfiguration.md) collection| Get a UserConfiguration object collection.|
|[Update](../api/mailfolder_update.md) | [MailFolder](mailfolder.md)	|Update MailFolder object. |
|[Delete](../api/mailfolder_delete.md) | None |Delete MailFolder object. |
|[Copy](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)||
|[Move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolderCount|Int32||
|DisplayName|String||
|Id|String| Read-only.|
|ParentFolderId|String||
|TotalItemCount|Int32||
|UnreadItemCount|Int32||
|WellKnownName|String||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|ChildFolders|[MailFolder](mailfolder.md) collection| Read-only. Nullable.|
|Messages|[Message](message.md) collection| Read-only. Nullable.|
|MultiValueExtendedProperties|[MultiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|SingleValueExtendedProperties|[SingleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| Read-only. Nullable.|
|UserConfigurations|[UserConfiguration](userconfiguration.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.MailFolder"
}-->

```json
{
  "ChildFolderCount": 1024,
  "DisplayName": "String",
  "Id": "String (identifier)",
  "ParentFolderId": "String",
  "TotalItemCount": 1024,
  "UnreadItemCount": 1024,
  "WellKnownName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "MailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->