---
uid: crmscript_ref_NSSelectionAgent_CreateSelectionFromSelection
title: NSSelectionEntity CreateSelectionFromSelection(Integer selectionId, String name, Integer targetSelectionType, Bool copyMembers)
intellisense: NSSelectionAgent.CreateSelectionFromSelection
keywords: NSSelectionAgent, CreateSelectionFromSelection
so.topic: reference
---

# NSSelectionEntity CreateSelectionFromSelection(Integer selectionId, String name, Integer targetSelectionType, Bool copyMembers)

Creates a new selection based on selection members from an existing selection.

**Parameters:**
 - **selectionId** The id of the selection to copy members from.
 - **name** The name of the new selection.
 - **targetSelectionType** The type of Selection to create. The type can be static or dynamic. If the original selection to copy from is static, the SelectionType can only be static. If the original selection is dynamic, both a static and dynamic selection can be created.
     - Enum: 0 = Static 
     - Enum: 1 = Dynamic 
     - Enum: 2 = Combined 
 - **copyMembers** If true, the members from the original selection will be added to the newly created selection.

**Returns:** NSSelectionEntity

```crmscript
NSSelectionAgent agent;
Integer selectionId;
String name;
Integer targetSelectionType;
Bool copyMembers;
NSSelectionEntity res = agent.CreateSelectionFromSelection(selectionId, name, targetSelectionType, copyMembers);
```

