---
title: triggerscripts
description: Trigger scripts
so.author: Christian Mogensen
so.date: 11.11.2020
keywords:
---

# TicketChangedTicketStatus (144)

Runs when a ticket is saved and status changed. If user-defined statuses are present in solution available values will differ from below.

## Input values
|Variable|Description|
|---|---|
| `entryId` | request ID|
| `ticketId` | request ID|
| `personId` | customer (person) ID|
| `contactId` | company (contact) ID|
| `ticketStatus.old` | old value|
| `ticketStatus.new` | new value|

## Ticket status

* Unknown = 0,
* Active = 1 - Request is currently active
* Closed = 2, Request has been closed
* Postponed = 3, Request has been postponed
* Deleted = 4, Request has been deleted
* Merged = 5, Request has been merged with another request

## Sample code

```crmscript
#setLanguageLevel 3;
String param1 = getVariable("ticketId");
```
