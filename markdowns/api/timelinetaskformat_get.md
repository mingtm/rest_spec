# Get TimelineTaskFormat

Retrieve the properties and relationships of timelinetaskformat object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /tasks/<id>/timelineFormat
GET /users/<objectId>/tasks/<id>/timelineFormat
GET /groups/<objectId>/tasks/<id>/timelineFormat
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. 
See relationships table of [TimelineTaskFormat](../resources/timelinetaskformat.md) object for supported names. |
|$select|string|Comma-separated list of properties to include in the response.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [TimelineTaskFormat](../resources/timelinetaskformat.md) object in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "timelinetaskformat"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 255
{
  "color": 99,
  "drawingStyle": "drawingStyle-value",
  "labelOffsetX": 99,
  "labelOffsetY": 99,
  "anchorPosition": "anchorPosition-value",
  "swimlane": 99,
  "calloutHeight": 99,
  "visible": true,
  "id": "id-value",
  "version": "version-value"
}
```

<!-- uuid: fca4a8cd-3a54-4098-b258-a878713f469a
2015-10-15 03:41:21 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TimelineTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->If successful, this method returns a `200 OK` response code and [TimelineTaskFormat](../resources/timelinetaskformat.md) object in the response body.