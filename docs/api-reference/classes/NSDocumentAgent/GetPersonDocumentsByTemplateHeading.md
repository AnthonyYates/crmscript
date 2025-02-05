---
uid: crmscript_ref_NSDocumentAgent_GetPersonDocumentsByTemplateHeading
title: NSDocument[] GetPersonDocumentsByTemplateHeading(Integer personId, Bool includeProjectDocuments, DateTime startTime, DateTime endTime, Integer count, Integer templateHeadingId)
intellisense: NSDocumentAgent.GetPersonDocumentsByTemplateHeading
keywords: NSDocumentAgent, GetPersonDocumentsByTemplateHeading
so.topic: reference
---

# NSDocument[] GetPersonDocumentsByTemplateHeading(Integer personId, Bool includeProjectDocuments, DateTime startTime, DateTime endTime, Integer count, Integer templateHeadingId)

Method that returns a specified number of document appointments within a time range, filtered by document template heading. The document appointments belong to the person specified. The heading represents a grouping or filtering of document templates.

**Parameters:**
 - **personId** The person id of the SuperOffice user (associate).
 - **includeProjectDocuments** If true, all appointments that belong to projects where the user is a project member are included as well as the appointments belonging to the person.
 - **startTime** The start of the time interval we want appointments from. This will usually be the current time.
 - **endTime** The end of the time interval.
 - **count** The maximum number of appointments that should be returned. -1 means no count restrictions.
 - **templateHeadingId** The document template heading id. The heading represents a grouping or filtering of document templates.

**Returns:** NSDocument[]

```crmscript
NSDocumentAgent agent;
Integer personId;
Bool includeProjectDocuments;
DateTime startTime;
DateTime endTime;
Integer count;
Integer templateHeadingId;
NSDocument[] res = agent.GetPersonDocumentsByTemplateHeading(personId, includeProjectDocuments, startTime, endTime, count, templateHeadingId);
```

