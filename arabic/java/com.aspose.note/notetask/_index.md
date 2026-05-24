---
title: "NoteTask"
second_title: "مرجع Aspose.Note for Java API"
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
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | إنشاء مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag وتاريخ الاستحقاق المحدد. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | * إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * إنشاء علامة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| [getDueDate()](#getDueDate--) | الحصول على تاريخ الاستحقاق أو تعيينه. |
| [getIcon()](#getIcon--) | يحصل أو يعيّن الأيقونة. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة للنوع. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | الحصول على تاريخ الاستحقاق أو تعيينه. |
| [setOpen()](#setOpen--) | تعيين العلامة إلى الحالة المفتوحة. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


إنشاء مهمة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag وتاريخ الاستحقاق المحدد.

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


* إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* إنشاء علامة ملاحظة جديدة مع أيقونة FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* إنشاء علامة ملاحظة جديدة مع أيقونة NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | الكائن. |

**Returns:**
منطقي - الـ `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن. |

**Returns:**
منطقي - الـ `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


الحصول على تاريخ الاستحقاق أو تعيينه.

القيمة: الـ `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


يحصل أو يعيّن الأيقونة.

القيمة: الـ [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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
عدد صحيح - الـ `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


الحصول على تاريخ الاستحقاق أو تعيينه.

القيمة: الـ `DateTime`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


تعيين العلامة إلى الحالة المفتوحة.

