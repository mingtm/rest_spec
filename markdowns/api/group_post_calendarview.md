# Create Event

Use this API to create a new Event.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Groups/<Id>/CalendarView
POST /me/JoinedGroups/<Id>/CalendarView
POST /Users/<Id>/JoinedGroups/<Id>/CalendarView

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Event](../resources/event.md) object.


### Response
If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/Groups/<Id>/CalendarView
Content-type: application/json
Content-length: 294

{
  "OriginalStartTimeZone": "OriginalStartTimeZone-value",
  "OriginalEndTimeZone": "OriginalEndTimeZone-value",
  "ResponseStatus": {
    "Response": "Response-value",
    "Time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "ReminderMinutesBeforeStart": 99,
  "IsReminderOn": true
}
```
In the request body, supply a JSON representation of [Event](../resources/event.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "OriginalStartTimeZone": "OriginalStartTimeZone-value",
  "OriginalEndTimeZone": "OriginalEndTimeZone-value",
  "ResponseStatus": {
    "Response": "Response-value",
    "Time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "ReminderMinutesBeforeStart": 99,
  "IsReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->