# Group resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get Group](../api/group_get.md) | [Group](group.md) |Read properties and relationships of group object.|
|[Create AcceptedSender](../api/group_post_acceptedsenders.md) |[DirectoryObject](directoryobject.md)| Create a new AcceptedSender by posting to the AcceptedSenders collection.|
|[List AcceptedSenders](../api/group_list_acceptedsenders.md) |[DirectoryObject](directoryobject.md) collection| Get a AcceptedSender object collection.|
|[Create Event](../api/group_post_calendarview.md) |[Event](event.md)| Create a new Event by posting to the CalendarView collection.|
|[List CalendarView](../api/group_list_calendarview.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Conversation](../api/group_post_conversations.md) |[Conversation](conversation.md)| Create a new Conversation by posting to the Conversations collection.|
|[List Conversations](../api/group_list_conversations.md) |[Conversation](conversation.md) collection| Get a Conversation object collection.|
|[Create Event](../api/group_post_events.md) |[Event](event.md)| Create a new Event by posting to the Events collection.|
|[List Events](../api/group_list_events.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Photo](../api/group_post_photos.md) |[Photo](photo.md)| Create a new Photo by posting to the Photos collection.|
|[List Photos](../api/group_list_photos.md) |[Photo](photo.md) collection| Get a Photo object collection.|
|[Create RejectedSender](../api/group_post_rejectedsenders.md) |[DirectoryObject](directoryobject.md)| Create a new RejectedSender by posting to the RejectedSenders collection.|
|[List RejectedSenders](../api/group_list_rejectedsenders.md) |[DirectoryObject](directoryobject.md) collection| Get a RejectedSender object collection.|
|[Create Subscription](../api/group_post_subscriptions.md) |[Subscription](subscription.md)| Create a new Subscription by posting to the Subscriptions collection.|
|[List Subscriptions](../api/group_list_subscriptions.md) |[Subscription](subscription.md) collection| Get a Subscription object collection.|
|[Create Thread](../api/group_post_threads.md) |[ConversationThread](conversationthread.md)| Create a new Thread by posting to the Threads collection.|
|[List Threads](../api/group_list_threads.md) |[ConversationThread](conversationthread.md) collection| Get a Thread object collection.|
|[Update](../api/group_update.md) | [Group](group.md)	|Update Group object. |
|[Delete](../api/group_delete.md) | None |Delete Group object. |
|[Addfavorite](../api/group_addfavorite.md)|None||
|[Removefavorite](../api/group_removefavorite.md)|None||
|[Resetunseencount](../api/group_resetunseencount.md)|None||
|[Subscribebymail](../api/group_subscribebymail.md)|None||
|[Unsubscribebymail](../api/group_unsubscribebymail.md)|None||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|AccessType|string| Possible values are: `None`, `Private`, `Secret`, `Public`.|
|AllowExternalSenders|Boolean||
|AutoSubscribeNewMembers|Boolean||
|Description|String||
|DisplayName|String||
|EmailAddress|String||
|Id|String| Read-only.|
|IsFavorite|Boolean||
|IsSubscribedByMail|Boolean||
|UnseenCount|Int32||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|AcceptedSenders|[DirectoryObject](directoryobject.md) collection| Read-only. Nullable.|
|Calendar|[Calendar](calendar.md)| Read-only. Nullable.|
|CalendarView|[Event](event.md) collection| Read-only. Nullable.|
|Conversations|[Conversation](conversation.md) collection| Read-only. Nullable.|
|Events|[Event](event.md) collection| Read-only. Nullable.|
|Photo|[Photo](photo.md)| Read-only. Nullable.|
|Photos|[Photo](photo.md) collection| Read-only. Nullable.|
|RejectedSenders|[DirectoryObject](directoryobject.md) collection| Read-only. Nullable.|
|Subscriptions|[Subscription](subscription.md) collection| Read-only. Nullable.|
|Threads|[ConversationThread](conversationthread.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Group"
}-->

```json
{
  "AccessType": "string",
  "AllowExternalSenders": true,
  "AutoSubscribeNewMembers": true,
  "Description": "String",
  "DisplayName": "String",
  "EmailAddress": "String",
  "Id": "String (identifier)",
  "IsFavorite": true,
  "IsSubscribedByMail": true,
  "UnseenCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->