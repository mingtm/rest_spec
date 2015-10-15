# Update the properties of directorylinkchange object.

Update the properties of directorylinkchange object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http

```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|associationType|String||
|deletionTimestamp|DateTimeOffset||
|objectType|String||
|sourceObjectId|String||
|sourceObjectType|String||
|sourceObjectUri|String||
|targetObjectId|String||
|targetObjectType|String||
|targetObjectUri|String||

### Response
If successful, this method returns a `200 OK` response code and updated [DirectoryLinkChange](../resources/directorylinkchange.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_directorylinkchange"
}-->
```http

Content-type: application/json
Content-length: 433
{
  "associationType": "associationType-value",
  "sourceObjectId": "sourceObjectId-value",
  "sourceObjectType": "sourceObjectType-value",
  "sourceObjectUri": "sourceObjectUri-value",
  "targetObjectId": "targetObjectId-value",
  "targetObjectType": "targetObjectType-value",
  "targetObjectUri": "targetObjectUri-value",
  "objectType": "objectType-value",
  "objectId": "objectId-value",
  "deletionTimestamp": "datetime-value"
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "directorylinkchange"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 433
{
  "associationType": "associationType-value",
  "sourceObjectId": "sourceObjectId-value",
  "sourceObjectType": "sourceObjectType-value",
  "sourceObjectUri": "sourceObjectUri-value",
  "targetObjectId": "targetObjectId-value",
  "targetObjectType": "targetObjectType-value",
  "targetObjectUri": "targetObjectUri-value",
  "objectType": "objectType-value",
  "objectId": "objectId-value",
  "deletionTimestamp": "datetime-value"
}
```

<!-- uuid: 18b87864-5e5c-4c09-b2ef-ebeb9e41410f
2015-10-15 03:41:18 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of directorylinkchange object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->