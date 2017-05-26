# User: ReminderView


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/ReminderView(StartDateTime=StartDateTime-value, EndDateTime=EndDateTime-value)
POST /Users/<Id>/ReminderView(StartDateTime=StartDateTime-value, EndDateTime=EndDateTime-value)

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request URL, provide following query parameters with values.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|StartDateTime|DateTime||
|EndDateTime|DateTime||

### Response
If successful, this method returns `200, OK` response code and [Reminder](../resources/reminder.md) collection object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
POST https://graph.microsoft.com/beta/me/ReminderView
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1025

{
  "value": [
    {
      "EventId": "EventId-value",
      "EventStartTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "EventEndTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "ChangeKey": "ChangeKey-value",
      "EventSubject": "EventSubject-value",
      "EventLocation": {
        "DisplayName": "DisplayName-value",
        "LocationEmailAddress": "LocationEmailAddress-value",
        "Address": {
          "Type": "Type-value",
          "PostOfficeBox": "PostOfficeBox-value",
          "Street": "Street-value",
          "City": "City-value",
          "State": "State-value",
          "CountryOrRegion": "CountryOrRegion-value",
          "PostalCode": "PostalCode-value"
        },
        "Coordinates": {
          "Altitude": 99,
          "Latitude": 99,
          "Longitude": 99,
          "Accuracy": 99,
          "AltitudeAccuracy": 99
        },
        "LocationUri": "LocationUri-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User: ReminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->