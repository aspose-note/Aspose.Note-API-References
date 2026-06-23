---
title: "NoteTask"
second_title: "مرجع Aspose.Note لـ Java API"
description: "يمثل مهمة ملاحظة."
type: docs
weight: 55
url: /ar/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

يمثل مهمة ملاحظة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | ينشئ مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag وتاريخ الاستحقاق المحدد. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | * ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * ينشئ علامة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [getDueDate()](#getDueDate--) | يحصل أو يضبط تاريخ الاستحقاق. |
| [getIcon()](#getIcon--) | يحصل أو يعيّن الأيقونة. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة للنوع. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | يحصل أو يضبط تاريخ الاستحقاق. |
| [setOpen()](#setOpen--) | يضبط العلامة إلى الحالة المفتوحة. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


ينشئ مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag وتاريخ الاستحقاق المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dueDate | java.util.Date | تاريخ الاستحقاق. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* ينشئ علامة ملاحظة جديدة مع أيقونة FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* ينشئ علامة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | الكائن. |

**Returns:**
منطقي - ال `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| كائن | java.lang.Object | الكائن. |

**Returns:**
منطقي - ال `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


يحصل أو يضبط تاريخ الاستحقاق.

القيمة: الـ `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


يحصل أو يعيّن الأيقونة.

القيمة: ال [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


يعمل كدالة تجزئة للنوع.

**Returns:**
عدد صحيح - ال `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


يحصل أو يضبط تاريخ الاستحقاق.

القيمة: الـ `DateTime`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


يضبط العلامة إلى الحالة المفتوحة.

