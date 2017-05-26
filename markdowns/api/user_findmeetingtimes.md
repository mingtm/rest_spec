# User: FindMeetingTimes


### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /me/FindMeetingTimes
POST /Users/<Id>/FindMeetingTimes

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
|Attendees|AttendeeBase||
|LocationConstraint|LocationConstraint||
|TimeConstraint|TimeConstraint||
|MeetingDuration|Duration||
|MaxCandidates|Int32||
|IsOrganizerOptional|Boolean||
|ReturnSuggestionHints|Boolean||

### Response
If successful, this method returns `200, OK` response code and [MeetingTimeCandidatesResult](../resources/meetingtimecandidatesresult.md) object in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/FindMeetingTimes
Content-type: application/json
Content-length: 743

{
  "Attendees": [
    {
      "Type": "Type-value"
    }
  ],
  "LocationConstraint": {
    "IsRequired": true,
    "SuggestLocation": true,
    "Locations": [
      {
        "ResolveAvailability": true
      }
    ]
  },
  "TimeConstraint": {
    "ActivityDomain": "ActivityDomain-value",
    "Timeslots": [
      {
        "Start": {
          "Date": "datetime-value",
          "Time": "datetime-value",
          "TimeZone": "TimeZone-value"
        },
        "End": {
          "Date": "datetime-value",
          "Time": "datetime-value",
          "TimeZone": "TimeZone-value"
        }
      }
    ]
  },
  "MeetingDuration": "datetime-value",
  "MaxCandidates": 99,
  "IsOrganizerOptional": true,
  "ReturnSuggestionHints": true
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.MeetingTimeCandidatesResult"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1449

{
  "MeetingTimeSlots": [
    {
      "MeetingTimeSlot": {
        "Start": {
          "Date": "datetime-value",
          "Time": "datetime-value",
          "TimeZone": "TimeZone-value"
        },
        "End": {
          "Date": "datetime-value",
          "Time": "datetime-value",
          "TimeZone": "TimeZone-value"
        }
      },
      "Confidence": 99,
      "OrganizerAvailability": "OrganizerAvailability-value",
      "AttendeeAvailability": [
        {
          "Attendee": {
            "Type": "Type-value"
          },
          "Availability": "Availability-value"
        }
      ],
      "Locations": [
        {
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
      ],
      "SuggestionHint": "SuggestionHint-value"
    }
  ],
  "EmptySuggestionsHint": "EmptySuggestionsHint-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User: FindMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->