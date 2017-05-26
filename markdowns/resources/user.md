# User resource type




### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get User](../api/user_get.md) | [User](user.md) |Read properties and relationships of user object.|
|[Create CalendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Create a new CalendarGroup by posting to the CalendarGroups collection.|
|[List CalendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) collection| Get a CalendarGroup object collection.|
|[Create Event](../api/user_post_calendarview.md) |[Event](event.md)| Create a new Event by posting to the CalendarView collection.|
|[List CalendarView](../api/user_list_calendarview.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Calendar](../api/user_post_calendars.md) |[Calendar](calendar.md)| Create a new Calendar by posting to the Calendars collection.|
|[List Calendars](../api/user_list_calendars.md) |[Calendar](calendar.md) collection| Get a Calendar object collection.|
|[Create ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Create a new ContactFolder by posting to the ContactFolders collection.|
|[List ContactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) collection| Get a ContactFolder object collection.|
|[Create Contact](../api/user_post_contacts.md) |[Contact](contact.md)| Create a new Contact by posting to the Contacts collection.|
|[List Contacts](../api/user_list_contacts.md) |[Contact](contact.md) collection| Get a Contact object collection.|
|[Create Drive](../api/user_post_drives.md) |[Drive](drive.md)| Create a new Drive by posting to the Drives collection.|
|[List Drives](../api/user_list_drives.md) |[Drive](drive.md) collection| Get a Drive object collection.|
|[Create Event](../api/user_post_events.md) |[Event](event.md)| Create a new Event by posting to the Events collection.|
|[List Events](../api/user_list_events.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Group](../api/user_post_joinedgroups.md) |[Group](group.md)| Create a new Group by posting to the JoinedGroups collection.|
|[List JoinedGroups](../api/user_list_joinedgroups.md) |[Group](group.md) collection| Get a Group object collection.|
|[Create MailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Create a new MailFolder by posting to the MailFolders collection.|
|[List MailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) collection| Get a MailFolder object collection.|
|[Create Message](../api/user_post_messages.md) |[Message](message.md)| Create a new Message by posting to the Messages collection.|
|[List Messages](../api/user_list_messages.md) |[Message](message.md) collection| Get a Message object collection.|
|[Create Person](../api/user_post_people.md) |[Person](person.md)| Create a new Person by posting to the People collection.|
|[List People](../api/user_list_people.md) |[Person](person.md) collection| Get a Person object collection.|
|[Create Photo](../api/user_post_photos.md) |[Photo](photo.md)| Create a new Photo by posting to the Photos collection.|
|[List Photos](../api/user_list_photos.md) |[Photo](photo.md) collection| Get a Photo object collection.|
|[Create Subscription](../api/user_post_subscriptions.md) |[Subscription](subscription.md)| Create a new Subscription by posting to the Subscriptions collection.|
|[List Subscriptions](../api/user_list_subscriptions.md) |[Subscription](subscription.md) collection| Get a Subscription object collection.|
|[Create TaskFolder](../api/user_post_taskfolders.md) |[TaskFolder](taskfolder.md)| Create a new TaskFolder by posting to the TaskFolders collection.|
|[List TaskFolders](../api/user_list_taskfolders.md) |[TaskFolder](taskfolder.md) collection| Get a TaskFolder object collection.|
|[Create TaskGroup](../api/user_post_taskgroups.md) |[TaskGroup](taskgroup.md)| Create a new TaskGroup by posting to the TaskGroups collection.|
|[List TaskGroups](../api/user_list_taskgroups.md) |[TaskGroup](taskgroup.md) collection| Get a TaskGroup object collection.|
|[Create Task](../api/user_post_tasks.md) |[Task](task.md)| Create a new Task by posting to the Tasks collection.|
|[List Tasks](../api/user_list_tasks.md) |[Task](task.md) collection| Get a Task object collection.|
|[Create WorkingWithEntity](../api/user_post_workingwithentities.md) |[WorkingWithEntity](workingwithentity.md)| Create a new WorkingWithEntity by posting to the WorkingWithEntities collection.|
|[List WorkingWithEntities](../api/user_list_workingwithentities.md) |[WorkingWithEntity](workingwithentity.md) collection| Get a WorkingWithEntity object collection.|
|[Update](../api/user_update.md) | [User](user.md)	|Update User object. |
|[Delete](../api/user_delete.md) | None |Delete User object. |
|[Findmeetingtimes](../api/user_findmeetingtimes.md)|[MeetingTimeCandidatesResult](meetingtimecandidatesresult.md)||
|[Getnotifications](../api/user_getnotifications.md)|[Notification](notification.md) collection||
|[Reminderview](../api/user_reminderview.md)|[Reminder](reminder.md) collection||
|[Sendmail](../api/user_sendmail.md)|None||
|[Trendingaround](../api/user_trendingaround.md)|[File](file.md)||
|[Workingwith](../api/user_workingwith.md)|[WorkingWithEntity](workingwithentity.md)||

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Alias|String||
|DisplayName|String||
|EmailAddress|String||
|Id|String| Read-only.|
|MailboxSettings|[MailboxSettings](mailboxsettings.md)||

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Calendar|[Calendar](calendar.md)| Read-only. Nullable.|
|CalendarGroups|[CalendarGroup](calendargroup.md) collection| Read-only. Nullable.|
|CalendarView|[Event](event.md) collection| Read-only. Nullable.|
|Calendars|[Calendar](calendar.md) collection| Read-only. Nullable.|
|ContactFolders|[ContactFolder](contactfolder.md) collection| Read-only. Nullable.|
|Contacts|[Contact](contact.md) collection| Read-only. Nullable.|
|Drives|[Drive](drive.md) collection| Read-only. Nullable.|
|Events|[Event](event.md) collection| Read-only. Nullable.|
|InferenceClassification|[InferenceClassification](inferenceclassification.md)| Read-only. Nullable.|
|JoinedGroups|[Group](group.md) collection| Read-only. Nullable.|
|MailFolders|[MailFolder](mailfolder.md) collection| Read-only. Nullable.|
|Messages|[Message](message.md) collection| Read-only. Nullable.|
|People|[Person](person.md) collection| Read-only. Nullable.|
|Photo|[Photo](photo.md)| Read-only. Nullable.|
|Photos|[Photo](photo.md) collection| Read-only. Nullable.|
|Subscriptions|[Subscription](subscription.md) collection| Read-only. Nullable.|
|TaskFolders|[TaskFolder](taskfolder.md) collection| Read-only. Nullable.|
|TaskGroups|[TaskGroup](taskgroup.md) collection| Read-only. Nullable.|
|Tasks|[Task](task.md) collection| Read-only. Nullable.|
|WorkingWithEntities|[WorkingWithEntity](workingwithentity.md) collection| Read-only. Nullable.|

### JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.User"
}-->

```json
{
  "Alias": "String",
  "DisplayName": "String",
  "EmailAddress": "String",
  "Id": "String (identifier)",
  "MailboxSettings": {"@odata.type": "microsoft.graph.MailboxSettings"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->