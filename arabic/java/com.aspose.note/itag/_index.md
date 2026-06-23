---
title: "ITag"
second_title: "مرجع Aspose.Note لـ Java API"
description: "الواجهة للعلامات من جميع الأنواع."
type: docs
weight: 109
url: /ar/java/com.aspose.note/itag/
---
```
public interface ITag
```

الواجهة للعلامات من جميع الأنواع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | يحصل على وقت الانتهاء. |
| [getCreationTime()](#getCreationTime--) | يحصل على وقت الإنشاء. |
| [getIcon()](#getIcon--) | يحصل على الأيقونة. |
| [getLabel()](#getLabel--) | يحصل على نص التسمية. |
| [getStatus()](#getStatus--) | يحصل على الحالة. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | يضبط وقت الإنشاء. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


يحصل على وقت الانتهاء.

القيمة: ال `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


يحصل على وقت الإنشاء.

القيمة: ال java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


يحصل على الأيقونة.

القيمة: ال [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


يحصل على نص التسمية.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


يحصل على الحالة.

القيمة: ال [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


يضبط وقت الإنشاء.

القيمة: ال java.util.Date.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

