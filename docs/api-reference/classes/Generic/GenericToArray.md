---
uid: crmscript_ref_Generic_GenericToArray_Generic_generic
title: Generic.GenericToArray(Generic generic)
intellisense: Generic.GenericToArray
langref: 1
sortOrder: 90
keywords: GenericToArray(Generic)
so.topic: reference
---

# Generic.GenericToArray(Generic generic)

Explicit downcast from a Generic to an array of Generic. If the generic does not represent an array, an exception is thrown. Typically, this function is used when traversing the members of a struct, and one of the members is an array. This can be tested with `getTypeDimensions()`, and then `GenericToArray()` can be used to access the sub-elements of the array for further (recursive) processing.

* **generic:** Generic The variable to downcast
* **Returns:** Generic[] The variable as an array
