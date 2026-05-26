---
title: "NoteTask"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een notitaak voor."
type: docs
weight: 55
url: /nl/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Stelt een notitaak voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Maakt een nieuwe notitaak met NoFollowUpDateFlag-pictogram en opgegeven vervaldatum. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Maakt een nieuwe notitag met FollowUpNextWeekFlag-pictogram. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Maakt een nieuwe notitag met FollowUpThisWeekFlag-pictogram. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Maakt een nieuwe notitag met FollowUpTodayFlag-pictogram. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Maakt een nieuwe notitag met FollowUpTomorrowFlag-pictogram. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Maakt een nieuwe notitag met NoFollowUpDateFlag-pictogram. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bepaalt of het opgegeven object gelijk is aan het huidige object. |
| [getDueDate()](#getDueDate--) | Haalt of stelt de vervaldatum in. |
| [getIcon()](#getIcon--) | Haalt het pictogram op of stelt dit in. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Dient als een hash-functie voor het type. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Haalt of stelt de vervaldatum in. |
| [setOpen()](#setOpen--) | Stelt de tag in op open status. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Maakt een nieuwe notitaak met NoFollowUpDateFlag-pictogram en opgegeven vervaldatum.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dueDate | java.util.Date | De vervaldatum. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Maakt een nieuwe notitag met FollowUpNextWeekFlag-pictogram.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Maakt een nieuwe notitag met FollowUpThisWeekFlag-pictogram.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Maakt een nieuwe notitag met FollowUpTodayFlag-pictogram.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Maakt een nieuwe notitag met FollowUpTomorrowFlag-pictogram.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Maakt een nieuwe notitag met NoFollowUpDateFlag-pictogram.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | Het object. |

**Returns:**
boolean - De `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bepaalt of het opgegeven object gelijk is aan het huidige object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object. |

**Returns:**
boolean - De `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Haalt of stelt de vervaldatum in.

Waarde: De `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Haalt het pictogram op of stelt dit in.

Waarde: De [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als een hash-functie voor het type.

**Returns:**
int - De `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Haalt of stelt de vervaldatum in.

Waarde: De `DateTime`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Stelt de tag in op open status.

