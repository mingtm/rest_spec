# AttendanceInfo resource type




### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|EmailAddress|String||
|EtaRequestStatus|String| Possible values are: `NoRequest`, `EtaRequestPending`, `EtaRequested`, `EtaResponseReceived`.|
|EtaRequestor|String||
|EtaResponse|String| Possible values are: `NoResponse`, `OnMyWay`, `BeThereIn5`, `BeThereIn10`, `StartWithoutMe`, `CantMakeIt`.|
|EtaResponseUrl|String||
|PhysicalPresence|String| Possible values are: `NoPresence`, `InRoom`, `LeftRoom`.|
|SkypePresence|String| Possible values are: `NoStatus`, `OnSkype`, `LeftSkype`.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.AttendanceInfo"
}-->

```json
{
  "EmailAddress": "String",
  "EtaRequestStatus": "String",
  "EtaRequestor": "String",
  "EtaResponse": "String",
  "EtaResponseUrl": "String",
  "PhysicalPresence": "String",
  "SkypePresence": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "AttendanceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->