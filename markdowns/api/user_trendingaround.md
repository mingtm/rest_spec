# User: TrendingAround


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/TrendingAround
POST /Users/<Id>/TrendingAround

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body

### Response
If successful, this method returns `200, OK` response code and [File](../resources/file.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_trendingaround"
}-->
```http
POST https://graph.microsoft.com/beta/me/TrendingAround
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.File"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 505

{
  "Name": "Name-value",
  "DateTimeCreated": "datetime-value",
  "DateTimeLastModified": "datetime-value",
  "WebUrl": "WebUrl-value",
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
  "description": "User: TrendingAround",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->