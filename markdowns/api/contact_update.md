# Update the properties of contact object.

Update the properties of contact object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/<objectId>/Contacts/<Id>
PATCH /drive/root/createdByUser/Contacts/<Id>
PATCH /drive/root/lastModifiedByUser/Contacts/<Id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AssistantName|String||
|Birthday|DateTimeOffset||
|BusinessAddress|PhysicalAddress||
|BusinessHomePage|String||
|BusinessPhones|String||
|Categories|String||
|ChangeKey|String||
|CompanyName|String||
|DateTimeCreated|DateTimeOffset||
|DateTimeLastModified|DateTimeOffset||
|Department|String||
|DisplayName|String||
|EmailAddresses|EmailAddress||
|FileAs|String||
|Generation|String||
|GivenName|String||
|HomeAddress|PhysicalAddress||
|HomePhones|String||
|ImAddresses|String||
|Initials|String||
|JobTitle|String||
|Manager|String||
|MiddleName|String||
|MobilePhone1|String||
|NickName|String||
|OfficeLocation|String||
|OtherAddress|PhysicalAddress||
|ParentFolderId|String||
|Profession|String||
|Surname|String||
|Title|String||
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
PUT /users/<objectId>/Contacts/<Id>
Content-type: application/json
Content-length: 1857
{
  "ParentFolderId": "ParentFolderId-value",
  "Birthday": "datetime-value",
  "FileAs": "FileAs-value",
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Initials": "Initials-value",
  "MiddleName": "MiddleName-value",
  "NickName": "NickName-value",
  "Surname": "Surname-value",
  "Title": "Title-value",
  "Generation": "Generation-value",
  "EmailAddresses": [
    {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  ],
  "ImAddresses": [
    "ImAddresses-value"
  ],
  "JobTitle": "JobTitle-value",
  "CompanyName": "CompanyName-value",
  "Department": "Department-value",
  "OfficeLocation": "OfficeLocation-value",
  "Profession": "Profession-value",
  "BusinessHomePage": "BusinessHomePage-value",
  "AssistantName": "AssistantName-value",
  "Manager": "Manager-value",
  "HomePhones": [
    "HomePhones-value"
  ],
  "BusinessPhones": [
    "BusinessPhones-value"
  ],
  "MobilePhone1": "MobilePhone1-value",
  "HomeAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "BusinessAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "OtherAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "YomiCompanyName": "YomiCompanyName-value",
  "YomiGivenName": "YomiGivenName-value",
  "YomiSurname": "YomiSurname-value",
  "ChangeKey": "ChangeKey-value",
  "Categories": [
    "Categories-value"
  ],
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "contact"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1857
{
  "ParentFolderId": "ParentFolderId-value",
  "Birthday": "datetime-value",
  "FileAs": "FileAs-value",
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Initials": "Initials-value",
  "MiddleName": "MiddleName-value",
  "NickName": "NickName-value",
  "Surname": "Surname-value",
  "Title": "Title-value",
  "Generation": "Generation-value",
  "EmailAddresses": [
    {
      "Name": "Name-value",
      "Address": "Address-value"
    }
  ],
  "ImAddresses": [
    "ImAddresses-value"
  ],
  "JobTitle": "JobTitle-value",
  "CompanyName": "CompanyName-value",
  "Department": "Department-value",
  "OfficeLocation": "OfficeLocation-value",
  "Profession": "Profession-value",
  "BusinessHomePage": "BusinessHomePage-value",
  "AssistantName": "AssistantName-value",
  "Manager": "Manager-value",
  "HomePhones": [
    "HomePhones-value"
  ],
  "BusinessPhones": [
    "BusinessPhones-value"
  ],
  "MobilePhone1": "MobilePhone1-value",
  "HomeAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "BusinessAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "OtherAddress": {
    "Street": "Street-value",
    "City": "City-value",
    "State": "State-value",
    "CountryOrRegion": "CountryOrRegion-value",
    "PostalCode": "PostalCode-value"
  },
  "YomiCompanyName": "YomiCompanyName-value",
  "YomiGivenName": "YomiGivenName-value",
  "YomiSurname": "YomiSurname-value",
  "ChangeKey": "ChangeKey-value",
  "Categories": [
    "Categories-value"
  ],
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```

<!-- uuid: db69b54f-7aa7-4631-9f90-3433311e8d92
2015-10-15 03:41:18 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of contact object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->