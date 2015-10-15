# Get permission

Retrieve the properties and relationships of permission object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/permissions/<id>
GET /drive/items/<id>/permissions/<id>
GET /drives/<id>/root/permissions/<id>
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. 
See relationships table of [permission](../resources/permission.md) object for supported names. |
|$select|string|Comma-separated list of properties to include in the response.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [permission](../resources/permission.md) object in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "permission"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762
{
  "grantedTo": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  },
  "id": "id-value",
  "invitation": {
    "email": "email-value",
    "redeemedBy": "redeemedBy-value",
    "signInRequired": true
  },
  "inheritedFrom": {
    "driveId": "driveId-value",
    "id": "id-value",
    "path": "path-value"
  },
  "link": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "type": "type-value",
    "webUrl": "webUrl-value"
  },
  "roles": [
    "roles-value"
  ],
  "shareId": "shareId-value"
}
```

<!-- uuid: c125e494-f1fb-4dc6-9991-3721ca8836fa
2015-10-15 03:41:20 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->If successful, this method returns a `200 OK` response code and [permission](../resources/permission.md) object in the response body.