# Create User

Use this API to create a new User.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /Users

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [User](../resources/user.md) object.


### Response
If successful, this method returns `201, Created` response code and [User](../resources/user.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/beta/Users
Content-type: application/json
Content-length: 732

{
  "EmailAddress": "EmailAddress-value",
  "DisplayName": "DisplayName-value",
  "Alias": "Alias-value",
  "MailboxSettings": {
    "AutomaticRepliesSetting": {
      "Status": "Status-value",
      "ExternalAudience": "ExternalAudience-value",
      "ScheduledStartDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "ScheduledEndDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "InternalReplyMessage": "InternalReplyMessage-value",
      "ExternalReplyMessage": "ExternalReplyMessage-value"
    },
    "TimeZone": "TimeZone-value",
    "Language": {
      "Locale": "Locale-value",
      "DisplayName": "DisplayName-value"
    }
  }
}
```
In the request body, supply a JSON representation of [User](../resources/user.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.User"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 752

{
  "EmailAddress": "EmailAddress-value",
  "DisplayName": "DisplayName-value",
  "Alias": "Alias-value",
  "MailboxSettings": {
    "AutomaticRepliesSetting": {
      "Status": "Status-value",
      "ExternalAudience": "ExternalAudience-value",
      "ScheduledStartDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "ScheduledEndDateTime": {
        "DateTime": {
        },
        "TimeZone": "TimeZone-value"
      },
      "InternalReplyMessage": "InternalReplyMessage-value",
      "ExternalReplyMessage": "ExternalReplyMessage-value"
    },
    "TimeZone": "TimeZone-value",
    "Language": {
      "Locale": "Locale-value",
      "DisplayName": "DisplayName-value"
    }
  },
  "Id": "Id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->