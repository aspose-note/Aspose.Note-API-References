---
title: "NoteTask"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt eine Notiz-Aufgabe dar."
type: docs
weight: 55
url: /de/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Stellt eine Notiz-Aufgabe dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Erstellt eine neue Notizaufgabe mit dem NoFollowUpDateFlag-Symbol und dem angegebenen Fälligkeitsdatum. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Erstellt ein neues Notiz-Tag mit dem FollowUpNextWeekFlag-Symbol. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Erstellt ein neues Notiz-Tag mit dem FollowUpThisWeekFlag-Symbol. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Erstellt ein neues Notiz-Tag mit dem FollowUpTodayFlag-Symbol. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Erstellt ein neues Notiz-Tag mit dem FollowUpTomorrowFlag-Symbol. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Erstellt ein neues Notiz-Tag mit dem NoFollowUpDateFlag-Symbol. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [getDueDate()](#getDueDate--) | Liest oder setzt das Fälligkeitsdatum. |
| [getIcon()](#getIcon--) | Liest oder setzt das Icon. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Dient als Hash-Funktion für den Typ. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Liest oder setzt das Fälligkeitsdatum. |
| [setOpen()](#setOpen--) | Setzt das Tag auf den offenen Zustand. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Erstellt eine neue Notizaufgabe mit dem NoFollowUpDateFlag-Symbol und dem angegebenen Fälligkeitsdatum.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dueDate | java.util.Date | Das Fälligkeitsdatum. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Erstellt ein neues Notiz-Tag mit dem FollowUpNextWeekFlag-Symbol.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Erstellt ein neues Notiz-Tag mit dem FollowUpThisWeekFlag-Symbol.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Erstellt ein neues Notiz-Tag mit dem FollowUpTodayFlag-Symbol.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Erstellt ein neues Notiz-Tag mit dem FollowUpTomorrowFlag-Symbol.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Erstellt ein neues Notiz-Tag mit dem NoFollowUpDateFlag-Symbol.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | Das Objekt. |

**Returns:**
boolean - Der `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt. |

**Returns:**
boolean - Der `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Liest oder setzt das Fälligkeitsdatum.

Wert: Das `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Liest oder setzt das Icon.

Wert: Das [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


Dient als Hash-Funktion für den Typ.

**Returns:**
int - Der `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Liest oder setzt das Fälligkeitsdatum.

Wert: Das `DateTime`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Setzt das Tag auf den offenen Zustand.

