# Create PimAlertInfo

Use this API to create a new PimAlertInfo.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /AlertInfo

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [PimAlertInfo](../resources/pimalertinfo.md) object.


### Response
If successful, this method returns `201, Created` response code and [PimAlertInfo](../resources/pimalertinfo.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_pimalertinfo_from_alertinfo"
}-->
```http
POST /AlertInfo
Content-type: application/json
```
In the request body, supply a JSON representation of [PimAlertInfo](../resources/pimalertinfo.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "pimalertinfo"
} -->
```http
HTTP/1.1 201 Created
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

<!-- uuid: 9e5a5008-04a4-4965-8d86-6f122649538d
2015-10-16 23:06:03 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create PimAlertInfo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->