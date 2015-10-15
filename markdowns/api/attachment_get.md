# Get Attachment

Retrieve the properties and relationships of attachment object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /users/<objectId>/Events/<Id>/Attachments/<Id>
GET /groups/<objectId>/Events/<Id>/Attachments/<Id>
GET /users/<objectId>/Messages/<Id>/Attachments/<Id>
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. 
See relationships table of [Attachment](../resources/attachment.md) object for supported names. |
|$select|string|Comma-separated list of properties to include in the response.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [Attachment](../resources/attachment.md) object in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "attachment"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162
{
  "Name": "Name-value",
  "ContentType": "ContentType-value",
  "Size": 99,
  "IsInline": true,
  "DateTimeLastModified": "datetime-value",
  "Id": "Id-value"
}
```

<!-- uuid: 8d9162fb-a84e-44cf-a9bf-1f0822c3bad1
2015-10-15 03:41:18 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->If successful, this method returns a `200 OK` response code and [Attachment](../resources/attachment.md) object in the response body.