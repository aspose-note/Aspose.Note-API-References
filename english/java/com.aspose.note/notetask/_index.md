---
title: NoteTask
second_title: Aspose.Note for Java API Reference
description: Represents a note task.
type: docs
weight: 45
url: /java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Represents a note task.
## Methods

| Method | Description |
| --- | --- |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Creates a new note tag with FollowUpNextWeekFlag icon. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Creates a new note tag with FollowUpThisWeekFlag icon. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Creates a new note tag with FollowUpTodayFlag icon. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Creates a new note tag with FollowUpTomorrowFlag icon. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Creates a new note tag with NoFollowUpDateFlag icon. |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Creates a new note task with NoFollowUpDateFlag icon and specified due date. |
| [getDueDate()](#getDueDate--) | Gets or sets the due date. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Gets or sets the due date. |
| [getIcon()](#getIcon--) | Gets or sets the icon. |
| [setOpen()](#setOpen--) | Sets the tag to open state. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the specified object is equal to the current object. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Determines whether the specified object is equal to the current object. |
| [hashCode()](#hashCode--) | Serves as a hash function for the type. |
| [getLabel()](#getLabel--) |  |
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Creates a new note tag with FollowUpNextWeekFlag icon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Creates a new note tag with FollowUpThisWeekFlag icon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Creates a new note tag with FollowUpTodayFlag icon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Creates a new note tag with FollowUpTomorrowFlag icon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Creates a new note tag with NoFollowUpDateFlag icon.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Creates a new note task with NoFollowUpDateFlag icon and specified due date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dueDate | java.util.Date | The due Date. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Gets or sets the due date.

Value: The  DateTime .

**Returns:**
java.util.Date
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Gets or sets the due date.

Value: The  DateTime .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getIcon() {#getIcon--}
```
public int getIcon()
```


Gets or sets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### setOpen() {#setOpen--}
```
public void setOpen()
```


Sets the tag to open state.

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object. |

**Returns:**
boolean - The  bool .
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Determines whether the specified object is equal to the current object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | The object. |

**Returns:**
boolean - The  bool .
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for the type.

**Returns:**
int - The  int .
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
