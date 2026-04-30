---
title: NoteTask
second_title: Aspose.Note for Java API Reference
description: Represents a note task.
type: docs
weight: 55
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
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Creates a new note task with NoFollowUpDateFlag icon and specified due date. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Creates a new note tag with FollowUpNextWeekFlag icon. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Creates a new note tag with FollowUpThisWeekFlag icon. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Creates a new note tag with FollowUpTodayFlag icon. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Creates a new note tag with FollowUpTomorrowFlag icon. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Creates a new note tag with NoFollowUpDateFlag icon. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Determines whether the specified object is equal to the current object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether the specified object is equal to the current object. |
| [getChecked()](#getChecked--) | Gets a value indicating whether the CheckBox is in the checked state. |
| [getClass()](#getClass--) |  |
| [getCompletedTime()](#getCompletedTime--) | Gets or sets the completed time. |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [getDueDate()](#getDueDate--) | Gets or sets the due date. |
| [getIcon()](#getIcon--) | Gets or sets the icon. |
| [getLabel()](#getLabel--) |  |
| [getStatus()](#getStatus--) | Gets or sets the status. |
| [hashCode()](#hashCode--) | Serves as a hash function for the type. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompleted()](#setCompleted--) | Sets the tag to completed state using current time as completed time. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Sets the tag to completed state. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Gets or sets the due date. |
| [setOpen()](#setOpen--) | Sets the tag to open state. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Gets a value indicating whether the CheckBox is in the checked state.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Gets or sets the completed time.

Value: The  Nullable\{DateTime\} .

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Gets or sets the creation time.

Value: The java.util.Date.

**Returns:**
java.util.Date
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Gets or sets the due date.

Value: The  DateTime .

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Gets or sets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Gets or sets the status.

Value: The [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Serves as a hash function for the type.

**Returns:**
int - The  int .
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Sets the tag to completed state using current time as completed time.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Sets the tag to completed state.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completedTime | java.util.Date | The completed time. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Gets or sets the creation time.

Value: The java.util.Date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

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

### setOpen() {#setOpen--}
```
public void setOpen()
```


Sets the tag to open state.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

