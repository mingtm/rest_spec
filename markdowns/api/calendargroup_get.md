# Get CalendarGroup

Retrieve the properties and relationships of calendargroup object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /users/<objectId>/CalendarGroups/<Id>
GET /drive/root/createdByUser/CalendarGroups/<Id>
GET /drive/root/lastModifiedByUser/CalendarGroups/<Id>
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. 
See relationships table of [CalendarGroup](../resources/calendargroup.md) object for supported names. |
|$select|string|Comma-separated list of properties to include in the response.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "calendargroup"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110
{
  "Name": "Name-value",
  "ChangeKey": "ChangeKey-value",
  "ClassId": "ClassId-value",
  "Id": "Id-value"
}
```

<!-- uuid: 9c41b667-aea1-4e2a-b01a-7c3796ace59c
2015-10-15 03:41:18 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->If successful, this method returns a `200 OK` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.