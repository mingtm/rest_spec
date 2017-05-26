# Create Person

Use this API to create a new Person.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/People
POST /Users/<Id>/People

```
### Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Workbook-Session-Id  | Workbook session Id that determines if changes are persisted or not. Optional.|

### Request body
In the request body, supply a JSON representation of [Person](../resources/person.md) object.


### Response
If successful, this method returns `201, Created` response code and [Person](../resources/person.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_person_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/People
Content-type: application/json
Content-length: 196

{
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Surname": "Surname-value",
  "Birthday": "Birthday-value",
  "PersonNotes": "PersonNotes-value",
  "IsFavorite": true
}
```
In the request body, supply a JSON representation of [Person](../resources/person.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Person"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 196

{
  "DisplayName": "DisplayName-value",
  "GivenName": "GivenName-value",
  "Surname": "Surname-value",
  "Birthday": "Birthday-value",
  "PersonNotes": "PersonNotes-value",
  "IsFavorite": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->