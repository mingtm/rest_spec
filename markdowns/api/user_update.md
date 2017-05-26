# Update user

Update the properties of user object.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /me
PATCH /Users/<Id>
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
|Alias|String||
|DisplayName|String||
|EmailAddress|String||
|MailboxSettings|MailboxSettings||

### Response
If successful, this method returns a `200 OK` response code and updated [User](../resources/user.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/beta/me
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
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.User"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->