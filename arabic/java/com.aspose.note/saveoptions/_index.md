---
title: "SaveOptions"
second_title: "مرجع Aspose.Note لـ Java API"
description: "فئة أساسية مجردة تمثل خيارات حفظ المستند لتنسيق معين."
type: docs
weight: 85
url: /ar/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

فئة أساسية مجردة تمثل خيارات حفظ المستند لتنسيق معين.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | يحصل أو يعيّن إعدادات الخط التي ستُستخدم أثناء الحفظ |
| [getPageCount()](#getPageCount--) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [getPageIndex()](#getPageIndex--) | يحصل أو يعيّن فهرس الصفحة الأولى التي سيتم حفظها. |
| [getSaveFormat()](#getSaveFormat--) | يحصل أو يعيّن التنسيق الذي يُحفظ به المستند. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | يحصل أو يعيّن إعدادات الخط التي ستُستخدم أثناء الحفظ |
| [setPageCount(int value)](#setPageCount-int-) | يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. |
| [setPageIndex(int value)](#setPageIndex-int-) | يحصل أو يعيّن فهرس الصفحة الأولى التي سيتم حفظها. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


يحصل أو يعيّن إعدادات الخط التي ستُستخدم أثناء الحفظ

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. بشكل افتراضي هو \{@link int\#Int32Extensions.MaxValue\} مما يعني أن جميع صفحات المستند سيتم عرضها.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


يحصل أو يعيّن فهرس الصفحة الأولى التي سيتم حفظها. بشكل افتراضي هو 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل أو يعيّن التنسيق الذي يُحفظ به المستند.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


يحصل أو يعيّن إعدادات الخط التي ستُستخدم أثناء الحفظ

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


يحصل أو يعيّن عدد الصفحات التي سيتم حفظها. بشكل افتراضي هو \{@link int\#Int32Extensions.MaxValue\} مما يعني أن جميع صفحات المستند سيتم عرضها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


يحصل أو يعيّن فهرس الصفحة الأولى التي سيتم حفظها. بشكل افتراضي هو 0.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

