# Update contact

Update the properties of contact object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/Contacts/<Id>
PATCH /Users/<Id>/Contacts/<Id>
PATCH /me/ContactFolders/<Id>/Contacts/<Id>
```
### Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AssistantName|String||
|Birthday|DateTimeOffset||
|Categories|String||
|ChangeKey|String||
|Children|String||
|CompanyName|String||
|CreatedDateTime|DateTimeOffset||
|Department|String||
|DisplayName|String||
|EmailAddresses|EmailAddress||
|FileAs|String||
|Flag|FollowupFlag||
|Gender|String||
|Generation|String||
|GivenName|String||
|ImAddresses|String||
|Initials|String||
|JobTitle|String||
|LastModifiedDateTime|DateTimeOffset||
|Manager|String||
|MiddleName|String||
|NickName|String||
|OfficeLocation|String||
|ParentFolderId|String||
|PersonalNotes|String||
|Phones|Phone||
|PostalAddresses|PhysicalAddress||
|Profession|String||
|SpouseName|String||
|Surname|String||
|Title|String||
|Websites|Website||
|WeddingAnniversary|Date||
|YomiCompanyName|String||
|YomiGivenName|String||
|YomiSurname|String||

### Response
If successful, this method returns a `200 OK` response code and updated [Contact](../resources/contact.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/Contacts/<Id>
Content-type: application/json
Content-length: 210

{
  "ParentFolderId": "ParentFolderId-value",
  "Birthday": "datetime-value",
  "FileAs": "FileAs-value",
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Initials": "Initials-value"
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "ParentFolderId": "ParentFolderId-value",
  "Birthday": "datetime-value",
  "FileAs": "FileAs-value",
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Initials": "Initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->