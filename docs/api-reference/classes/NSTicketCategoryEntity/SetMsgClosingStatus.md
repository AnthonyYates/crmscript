---
uid: crmscript_ref_NSTicketCategoryEntity_SetMsgClosingStatus
title: SetMsgClosingStatus(Integer msgClosingStatus)
intellisense: NSTicketCategoryEntity.SetMsgClosingStatus
keywords: NSTicketCategoryEntity, GetMsgClosingStatus
so.topic: reference
---

# SetMsgClosingStatus(Integer msgClosingStatus)

An integer indicating if new messages should have the &apos;close request&apos; in this category checked as default, or if the users preferences should be selected.

**Parameter:** 
 - **msgClosingStatus** Integer
     - Enum: 0 = UserDefined 
     - Enum: 1 = Active 
     - Enum: 2 = Closed 
     - Enum: 3 = Postponed 

```crmscript
NSTicketCategoryEntity thing;
Integer msgClosingStatus;
thing.SetMsgClosingStatus(msgClosingStatus);
```

