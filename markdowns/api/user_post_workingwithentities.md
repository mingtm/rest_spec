# Create WorkingWithEntity

Use this API to create a new WorkingWithEntity.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/WorkingWithEntities
POST /Users/<Id>/WorkingWithEntities

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [WorkingWithEntity](../resources/workingwithentity.md) object.


### Response
If successful, this method returns `201, Created` response code and [WorkingWithEntity](../resources/workingwithentity.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workingwithentity_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/WorkingWithEntities
Content-type: application/json
Content-length: 418

{
  "PreferredName": "PreferredName-value",
  "Email": "Email-value",
  "EntityACL": {
    "AccessControlEntries": [
      {
        "AccessRight": "AccessRight-value",
        "AccessType": "AccessType-value",
        "Claim": {
          "Type": "Type-value",
          "Value": "Value-value",
          "ValueType": "ValueType-value",
          "OriginalIssuer": "OriginalIssuer-value"
        }
      }
    ]
  }
}
```
In the request body, supply a JSON representation of [WorkingWithEntity](../resources/workingwithentity.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.WorkingWithEntity"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 438

{
  "PreferredName": "PreferredName-value",
  "Email": "Email-value",
  "EntityACL": {
    "AccessControlEntries": [
      {
        "AccessRight": "AccessRight-value",
        "AccessType": "AccessType-value",
        "Claim": {
          "Type": "Type-value",
          "Value": "Value-value",
          "ValueType": "ValueType-value",
          "OriginalIssuer": "OriginalIssuer-value"
        }
      }
    ]
  },
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create WorkingWithEntity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->