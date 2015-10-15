# Update the properties of contactfolder object.

Update the properties of contactfolder object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/<objectId>/ContactFolders/<Id>
PATCH /drive/root/createdByUser/ContactFolders/<Id>
PATCH /drive/root/lastModifiedByUser/ContactFolders/<Id>
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|DisplayName|String||
|ParentFolderId|String||

### Response
If successful, this method returns a `200 OK` response code and updated [ContactFolder](../resources/contactfolder.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PUT /users/<objectId>/ContactFolders/<Id>
Content-type: application/json
Content-length: 104
{
  "ParentFolderId": "ParentFolderId-value",
  "DisplayName": "DisplayName-value",
  "Id": "Id-value"
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "contactfolder"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104
{
  "ParentFolderId": "ParentFolderId-value",
  "DisplayName": "DisplayName-value",
  "Id": "Id-value"
}
```

<!-- uuid: d0a60a1b-7584-4d4e-bcee-79f8b46c76a2
2015-10-15 03:41:18 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of contactfolder object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->