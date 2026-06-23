---
title: "CheckBox"
second_title: "مرجع Aspose.Note لـ Java API"
description: "الفئة الأساسية للوسوم التي يمكنها تبديل حالتها بين مكتملة وغير مكتملة."
type: docs
weight: 13
url: /ar/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

الفئة الأساسية للوسوم التي يمكنها تبديل حالتها بين مكتملة وغير مكتملة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getChecked()](#getChecked--) | يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة. |
| [getCompletedTime()](#getCompletedTime--) | يحصل أو يعيّن وقت الانتهاء. |
| [getCreationTime()](#getCreationTime--) | يحصل أو يعيّن وقت الإنشاء. |
| [getIcon()](#getIcon--) | يحصل أو يعيّن الأيقونة. |
| [getStatus()](#getStatus--) | يحصل أو يعيّن الحالة. |
| [setCompleted()](#setCompleted--) | يضبط العلامة إلى الحالة المكتملة باستخدام الوقت الحالي كوقت إكمال. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | يضبط العلامة إلى الحالة المكتملة. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | يحصل أو يعيّن وقت الإنشاء. |
| [setOpen()](#setOpen--) | يضبط العلامة إلى الحالة المفتوحة. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


يحصل على قيمة تشير إلى ما إذا كان CheckBox في الحالة المحددة.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


يحصل أو يعيّن وقت الانتهاء.

القيمة: ال `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


يحصل أو يعيّن وقت الإنشاء.

القيمة: ال java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


يحصل أو يعيّن الأيقونة.

القيمة: ال [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


يحصل أو يعيّن الحالة.

القيمة: ال [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


يضبط العلامة إلى الحالة المكتملة باستخدام الوقت الحالي كوقت إكمال.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


يضبط العلامة إلى الحالة المكتملة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| completedTime | java.util.Date | وقت الإكمال. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


يحصل أو يعيّن وقت الإنشاء.

القيمة: ال java.util.Date.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


يضبط العلامة إلى الحالة المفتوحة.

