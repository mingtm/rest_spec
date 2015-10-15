# Update the properties of privilegedrole object.

Update the properties of privilegedrole object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /PrivilegedRoles/<Id>
PATCH /PrivilegedRoleAssignments/<UserId|RoleId>/RoleInfo
```
### Optional request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Name|String||

### Response
If successful, this method returns a `200 OK` response code and updated [PrivilegedRole](../resources/privilegedrole.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_privilegedrole"
}-->
```http
PUT /PrivilegedRoles/<Id>
Content-type: application/json
Content-length: 46
{
  "Id": "Id-value",
  "Name": "Name-value"
}
```
##### Response
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "privilegedrole"
} -->
Here is an example of the response.
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46
{
  "Id": "Id-value",
  "Name": "Name-value"
}
```

<!-- uuid: 449e74f1-fa54-407c-8a8e-f76020270e2d
2015-10-15 03:41:20 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update the properties of privilegedrole object.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->