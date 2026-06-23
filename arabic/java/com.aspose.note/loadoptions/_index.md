---
title: "LoadOptions"
second_title: "مرجع Aspose.Note لـ Java API"
description: "الخيارات المستخدمة لتحميل مستند."
type: docs
weight: 46
url: /ar/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

الخيارات المستخدمة لتحميل مستند.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | يُنشئ مثيلًا جديدًا للفئة `LoadOptions`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | يحصل أو يعيّن كلمة مرور لمحتوى المستند المشفر. |
| [getLoadHistory()](#getLoadHistory--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان محمّل المستند يجب أن يتجاهل السجل. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | يحصل أو يعيّن كلمة مرور لمحتوى المستند المشفر. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كان محمّل المستند يجب أن يتجاهل السجل. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


يُنشئ مثيلًا جديدًا للفئة `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


يحصل أو يعيّن كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حال عدم حماية المستند بكلمة مرور.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان محمّل المستند يجب أن يتجاهل السجل. استخدم هذا الخيار لتقليل استهلاك الذاكرة والمعالج. القيمة الافتراضية هي `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


يحصل أو يعيّن كلمة مرور لمحتوى المستند المشفر. يتم تجاهل القيمة في حال عدم حماية المستند بكلمة مرور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كان محمّل المستند يجب أن يتجاهل السجل. استخدم هذا الخيار لتقليل استهلاك الذاكرة والمعالج. القيمة الافتراضية هي `true`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

