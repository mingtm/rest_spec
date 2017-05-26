# Create Subscription

Use this API to create a new Subscription.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Groups/<Id>/Subscriptions
POST /me/JoinedGroups/<Id>/Subscriptions
POST /Users/<Id>/JoinedGroups/<Id>/Subscriptions

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Subscription](../resources/subscription.md) object.


### Response
If successful, this method returns `201, Created` response code and [Subscription](../resources/subscription.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/Groups/<Id>/Subscriptions
Content-type: application/json
Content-length: 70

{
  "Resource": "Resource-value",
  "ChangeType": "ChangeType-value"
}
```
In the request body, supply a JSON representation of [Subscription](../resources/subscription.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Subscription"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 90

{
  "Resource": "Resource-value",
  "ChangeType": "ChangeType-value",
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->