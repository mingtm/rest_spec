# Create Task

Use this API to create a new Task.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Tasks
POST /Users/<Id>/Tasks

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Task](../resources/task.md) object.


### Response
If successful, this method returns `201, Created` response code and [Task](../resources/task.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_task_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/Tasks
Content-type: application/json
Content-length: 356

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
```
In the request body, supply a JSON representation of [Task](../resources/task.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Task"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 356

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->