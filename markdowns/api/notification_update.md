# Update notification

Update the properties of notification object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http

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
|ChangeType|string| Possible values are: `Created`, `Updated`, `Deleted`, `Acknowledgment`, `Missed`.|
|Resource|String||
|ResourceCount|Int32||
|SequenceNumber|Int32||
|SubscriptionExpirationDateTime|DateTimeOffset||
|SubscriptionId|String||

### Response
If successful, this method returns a `200 OK` response code and updated [Notification](../resources/notification.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_notification"
}-->
```http

Content-type: application/json
Content-length: 215

{
  "SubscriptionId": "SubscriptionId-value",
  "SubscriptionExpirationDateTime": "datetime-value",
  "SequenceNumber": 99,
  "ChangeType": "ChangeType-value",
  "Resource": "Resource-value",
  "ResourceCount": 99
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Notification"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "SubscriptionId": "SubscriptionId-value",
  "SubscriptionExpirationDateTime": "datetime-value",
  "SequenceNumber": 99,
  "ChangeType": "ChangeType-value",
  "Resource": "Resource-value",
  "ResourceCount": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update notification",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->