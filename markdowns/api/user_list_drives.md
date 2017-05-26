# List Drives

Retrieve a list of drive objects.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /me/Drives
GET /Users/<Id>/Drives
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->
```http
GET https://graph.microsoft.com/beta/me/Drives
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 459

{
  "value": [
    {
      "Id": "Id-value",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List Drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->