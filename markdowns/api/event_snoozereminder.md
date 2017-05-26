# Event: SnoozeReminder


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/Events/<Id>/SnoozeReminder
POST /me/CalendarView/<Id>/SnoozeReminder
POST /Users/<Id>/Events/<Id>/SnoozeReminder

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|NewReminderTime|DateTimeTimeZone||

### Response
If successful, this method returns `200, OK` response code. It does not return anything in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/Events/<Id>/SnoozeReminder
Content-type: application/json
Content-length: 88

{
  "NewReminderTime": {
    "DateTime": {
    },
    "TimeZone": "TimeZone-value"
  }
}
```

##### Response
Here is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Event: SnoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->