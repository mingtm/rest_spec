# User: GetNotifications


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/GetNotifications
POST /Users/<Id>/GetNotifications

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
|ConnectionTimeoutInMinutes|Int32||
|KeepAliveNotificationIntervalInSeconds|Int32||
|SubscriptionIds|String||

### Response
If successful, this method returns `200, OK` response code and [Notification](../resources/notification.md) collection object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_getnotifications"
}-->
```http
POST https://graph.microsoft.com/beta/me/GetNotifications
Content-type: application/json
Content-length: 142

{
  "ConnectionTimeoutInMinutes": 99,
  "KeepAliveNotificationIntervalInSeconds": 99,
  "SubscriptionIds": [
    "SubscriptionIds-value"
  ]
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Notification",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 268

{
  "value": [
    {
      "SubscriptionId": "SubscriptionId-value",
      "SubscriptionExpirationDateTime": "datetime-value",
      "SequenceNumber": 99,
      "ChangeType": "ChangeType-value",
      "Resource": "Resource-value",
      "ResourceCount": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User: GetNotifications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->