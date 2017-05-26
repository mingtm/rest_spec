# Task: Complete


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Tasks/<Id>/Complete
POST /Users/<Id>/Tasks/<Id>/Complete
POST /me/TaskFolders/<Id>/Tasks/<Id>/Complete

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body

### Response
If successful, this method returns `200, OK` response code and [Task](../resources/task.md) collection object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "task_complete"
}-->
```http
POST https://graph.microsoft.com/beta/me/Tasks/<Id>/Complete
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Task",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 453

{
  "value": [
    {
      "AssignedTo": "AssignedTo-value",
      "Body": {
        "ContentType": "ContentType-value",
        "Content": "Content-value"
      },
      "CompletedDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "DueDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "Importance": "Importance-value",
      "IsReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Task: Complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->