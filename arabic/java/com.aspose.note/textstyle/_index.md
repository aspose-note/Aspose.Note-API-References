---
title: "TextStyle"
second_title: "مرجع Aspose.Note for Java API"
description: "يحدد نمط النص."
type: docs
weight: 93
url: /ar/java/com.aspose.note/textstyle/
---

**Inheritance:**
java.lang.Object, com.aspose.note.Style
```
public final class TextStyle extends Style<TextStyle>
```

يحدد نمط النص.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [TextStyle()](#TextStyle--) | يقوم بتهيئة نسخة جديدة من الفئة `TextStyle`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(TextStyle other)](#equals-com.aspose.note.TextStyle-) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي. |
| [getDefault()](#getDefault--) | يحصل على النمط مع الثقافة "en-US". |
| [getDefaultMsOneNoteTitleDateStyle()](#getDefaultMsOneNoteTitleDateStyle--) | يحصل على النمط الافتراضي لتاريخ العنوان في MS OneNote. |
| [getDefaultMsOneNoteTitleTextStyle()](#getDefaultMsOneNoteTitleTextStyle--) | يحصل على النمط الافتراضي لنص العنوان في MS OneNote. |
| [getDefaultMsOneNoteTitleTimeStyle()](#getDefaultMsOneNoteTitleTimeStyle--) | يحصل على النمط الافتراضي لوقت العنوان في MS OneNote. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | يحصل على عنوان الارتباط التشعبي. |
| [getLanguage()](#getLanguage--) | يحصل على لغة النص. |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة للنوع. |
| [isHidden()](#isHidden--) | يحصل على قيمة تشير إلى ما إذا كان نمط النص مخفيًا. |
| [isHyperlink()](#isHyperlink--) | يحصل على قيمة تشير إلى ما إذا كان نمط النص ارتباطًا تشعبيًا. |
| [isMathFormatting()](#isMathFormatting--) | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص بتنسيق رياضي. |
| [setHidden(boolean value)](#setHidden-boolean-) | يضبط قيمة تشير إلى ما إذا كان نمط النص مخفيًا. |
| [setHyperlink(boolean value)](#setHyperlink-boolean-) | يضبط قيمة تشير إلى ما إذا كان نمط النص ارتباطًا تشعبيًا. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | يضبط عنوان الارتباط التشعبي. |
| [setLanguage(Locale value)](#setLanguage-java.util.Locale-) | يضبط لغة النص. |
| [setMathFormatting(boolean value)](#setMathFormatting-boolean-) | يضبط قيمة تشير إلى ما إذا كان نمط النص هو تنسيق رياضي. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


يقوم بتهيئة نسخة جديدة من الفئة `TextStyle`.

### equals(TextStyle other) {#equals-com.aspose.note.TextStyle-}
```
public boolean equals(TextStyle other)
```


يحدد ما إذا كان الكائن المحدد مساويًا للكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [TextStyle](../../com.aspose.note/textstyle) | الكائن. |

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
### getDefault() {#getDefault--}
```
public static TextStyle getDefault()
```


يحصل على النمط مع الثقافة "en-US".

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleDateStyle() {#getDefaultMsOneNoteTitleDateStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleDateStyle()
```


يحصل على النمط الافتراضي لتاريخ العنوان في MS OneNote.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTextStyle() {#getDefaultMsOneNoteTitleTextStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTextStyle()
```


يحصل على النمط الافتراضي لنص العنوان في MS OneNote.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTimeStyle() {#getDefaultMsOneNoteTitleTimeStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTimeStyle()
```


يحصل على النمط الافتراضي لوقت العنوان في MS OneNote.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public String getHyperlinkAddress()
```


يحصل على عنوان الارتباط التشعبي. يجب تعيينه إذا كانت قيمة الخاصية [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) صحيحة.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public Locale getLanguage()
```


يحصل على لغة النص.

**Returns:**
java.util.Locale
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة للنوع.

**Returns:**
عدد صحيح - الـ `int`.
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يحصل على قيمة تشير إلى ما إذا كان نمط النص مخفيًا.

**Returns:**
boolean
### isHyperlink() {#isHyperlink--}
```
public boolean isHyperlink()
```


يحصل على قيمة تشير إلى ما إذا كان نمط النص ارتباطًا تشعبيًا.

**Returns:**
boolean
### isMathFormatting() {#isMathFormatting--}
```
public boolean isMathFormatting()
```


يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص بتنسيق رياضي.

**Returns:**
boolean
### setHidden(boolean value) {#setHidden-boolean-}
```
public TextStyle setHidden(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان نمط النص مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlink(boolean value) {#setHyperlink-boolean-}
```
public TextStyle setHyperlink(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان نمط النص ارتباطًا تشعبيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public TextStyle setHyperlinkAddress(String value)
```


يضبط عنوان الارتباط التشعبي. يجب تعيينه إذا كانت قيمة الخاصية [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) صحيحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setLanguage(Locale value) {#setLanguage-java.util.Locale-}
```
public TextStyle setLanguage(Locale value)
```


يضبط لغة النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Locale |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setMathFormatting(boolean value) {#setMathFormatting-boolean-}
```
public TextStyle setMathFormatting(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان نمط النص هو تنسيق رياضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
