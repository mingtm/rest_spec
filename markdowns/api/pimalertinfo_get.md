# Get PimAlertInfo

Retrieve the properties and relationships of pimalertinfo object.
### Prerequisites
The following **scopes** are required to execute this API: ### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /AlertInfo/<AlertId>
```
### Optional query parameters
|Name|Value|Description|
|:---------------|:--------|:-------|
|$count|none|The count of related entities can be requested by specifying the $count query option.|
|$expand|string|Comma-separated list of relationships to expand and include in the response. 
See relationships table of [PimAlertInfo](../resources/pimalertinfo.md) object for supported names. |
|$select|string|Comma-separated list of properties to include in the response.|

### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| X-Sample-Header  | string  | Sample of how the HTTP header. Update accordingly...|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [PimAlertInfo](../resources/pimalertinfo.md) object in the response body.
### Example
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "pimalertinfo"
} -->
```json
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370
{
  "AlertId": "AlertId-value",
  "AlertName": "AlertName-value",
  "AlertDescription": "AlertDescription-value",
  "LowSeverityThreshold": 99,
  "MediumSeverityThreshold": 99,
  "HighSeverityThreshold": 99,
  "Type": 99,
  "Severity": 99,
  "SecurityImpact": "SecurityImpact-value",
  "MitigationSteps": "MitigationSteps-value",
  "HowToPrevent": "HowToPrevent-value"
}
```

<!-- uuid: 7fc9c13a-6a5f-423c-8152-1d6de711d432
2015-10-15 03:41:20 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get PimAlertInfo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->If successful, this method returns a `200 OK` response code and [PimAlertInfo](../resources/pimalertinfo.md) object in the response body.