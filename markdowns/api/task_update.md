# Update task

Update the properties of task object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/Tasks/<Id>
PATCH /Users/<Id>/Tasks/<Id>
PATCH /me/TaskFolders/<Id>/Tasks/<Id>
```
### Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AssignedTo|String||
|Body|ItemBody||
|Categories|String||
|ChangeKey|String||
|CompletedDateTime|DateTimeTimeZone||
|CreatedDateTime|DateTimeOffset||
|DueDateTime|DateTimeTimeZone||
|Importance|string| Possible values are: `Low`, `Normal`, `High`.|
|IsReminderOn|Boolean||
|LastModifiedDateTime|DateTimeOffset||
|Owner|String||
|ParentFolderId|String||
|Recurrence|PatternedRecurrence||
|ReminderDateTime|DateTimeTimeZone||
|StartDateTime|DateTimeTimeZone||
|Status|string| Possible values are: `NotStarted`, `InProgress`, `Completed`, `WaitingOnOthers`, `Deferred`.|
|Subject|String||

### Response
If successful, this method returns a `200 OK` response code and updated [Task](../resources/task.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_task"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/Tasks/<Id>
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
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Task"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->