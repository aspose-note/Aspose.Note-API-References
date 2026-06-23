---
title: "NotebookSaveOptions"
second_title: "مرجع Aspose.Note لـ Java API"
description: "فئة أساسية مجردة تمثل خيارات حفظ دفتر الملاحظات لتنسيق معين."
type: docs
weight: 61
url: /ar/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

فئة أساسية مجردة تمثل خيارات حفظ دفتر الملاحظات لتنسيق معين.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان يجب حفظ مستندات الأطفال صراحةً. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | يحصل على خيارات الحفظ لجميع مستندات الأطفال في الدفتر. |
| [getFlatten()](#getFlatten--) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على الصيغة التي يُحفظ بها الدفتر. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان يجب حفظ مستندات الأطفال صراحةً. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | يحصل على أو يضبط قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


يحصل على أو يضبط قيمة تشير إلى ما إذا كان يجب حفظ مستندات الأطفال صراحةً.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم حفظ المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أن المستخدم يجب أن يحفظ كل عقدة فرعية للمفكرة بشكل صريح. إذا كانت المفكرة تُحفظ إلى تدفق، فإن القيمة تكون دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


يحصل على خيارات الحفظ لجميع مستندات الأطفال في الدفتر.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


يحصل على أو يضبط قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


يحصل على الصيغة التي يُحفظ بها الدفتر.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


يحصل على أو يضبط قيمة تشير إلى ما إذا كان يجب حفظ مستندات الأطفال صراحةً.

--------------------

القيمة الافتراضية هي `false`، لذا سيتم حفظ المستندات الفرعية ضمنيًا. القيمة `true` تشير إلى أن المستخدم يجب أن يحفظ كل عقدة فرعية للمفكرة بشكل صريح. إذا كانت المفكرة تُحفظ إلى تدفق، فإن القيمة تكون دائمًا `true` رغم أنه تم تعيينها صراحةً من قبل المستخدم إلى `false`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


يحصل على أو يضبط قيمة تشير إلى ما إذا كان هيكل الأطفال في الدفتر يُحفظ مسطحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

