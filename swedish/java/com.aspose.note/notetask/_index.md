---
title: "NoteTask"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en notuppgift."
type: docs
weight: 55
url: /sv/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Representerar en notuppgift.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Skapar en ny notuppgift med NoFollowUpDateFlag-ikon och angivet förfallodatum. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Skapar en ny nottagg med FollowUpNextWeekFlag-ikon. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Skapar en ny nottagg med FollowUpThisWeekFlag-ikon. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Skapar en ny nottagg med FollowUpTodayFlag-ikon. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Skapar en ny nottagg med FollowUpTomorrowFlag-ikon. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Skapar en ny nottagg med NoFollowUpDateFlag-ikon. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om det angivna objektet är lika med det aktuella objektet. |
| [getDueDate()](#getDueDate--) | Hämtar eller anger förfallodatumet. |
| [getIcon()](#getIcon--) | Hämtar eller anger ikonen. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Fungerar som en hash-funktion för typen. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Hämtar eller anger förfallodatumet. |
| [setOpen()](#setOpen--) | Sätter taggen till öppet läge. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Skapar en ny notuppgift med NoFollowUpDateFlag-ikon och angivet förfallodatum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dueDate | java.util.Date | Förfallodatumet. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Skapar en ny nottagg med FollowUpNextWeekFlag-ikon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Skapar en ny nottagg med FollowUpThisWeekFlag-ikon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Skapar en ny nottagg med FollowUpTodayFlag-ikon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Skapar en ny nottagg med FollowUpTomorrowFlag-ikon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Skapar en ny nottagg med NoFollowUpDateFlag-ikon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Bestämmer om det angivna objektet är lika med det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | Objektet. |

**Returns:**
boolean - `bool`-typen.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestämmer om det angivna objektet är lika med det aktuella objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet. |

**Returns:**
boolean - `bool`-typen.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Hämtar eller anger förfallodatumet.

Värde: Den `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Hämtar eller anger ikonen.

Värde: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


Fungerar som en hash-funktion för typen.

**Returns:**
int - `int`-typen.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Hämtar eller anger förfallodatumet.

Värde: Den `DateTime`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Sätter taggen till öppet läge.

