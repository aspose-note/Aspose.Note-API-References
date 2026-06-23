---
title: "NumberList"
second_title: "مرجع Aspose.Note لـ Java API"
description: "يمثل القائمة المرقمة أو ذات النقاط."
type: docs
weight: 64
url: /ar/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

يمثل القائمة المرقمة أو ذات النقاط.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | ينشئ مثيلاً جديداً لفئة `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | ينشئ مثيلاً جديداً لفئة `NumberList`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي. |
| [getFont()](#getFont--) | يحصل أو يعيّن اسم الخط. |
| [getFontColor()](#getFontColor--) | يحصل أو يعيّن لون الخط. |
| [getFontSize()](#getFontSize--) | يحصل أو يضبط حجم الخط. |
| [getFormat()](#getFormat--) | يحصل أو يعيّن تنسيق رأس السطر. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يعيّن وقت التعديل الأخير. |
| [getNumberFormat()](#getNumberFormat--) | يحصل أو يعيّن تنسيق الرقم المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | يحصل على رأس القائمة المرقمة. |
| [getRestart()](#getRestart--) | يحصل أو يعيّن القيمة الرقمية التي تتجاوز القيمة العددية التلقائية لعنصر القائمة. |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة للنوع. |
| [isBold()](#isBold--) | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص غامقًا. |
| [isItalic()](#isItalic--) | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا. |
| [setBold(boolean value)](#setBold-boolean-) | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص غامقًا. |
| [setFont(String value)](#setFont-java.lang.String-) | يحصل أو يعيّن اسم الخط. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | يحصل أو يعيّن لون الخط. |
| [setFontSize(int value)](#setFontSize-int-) | يحصل أو يضبط حجم الخط. |
| [setFormat(String value)](#setFormat-java.lang.String-) | يحصل أو يعيّن تنسيق رأس السطر. |
| [setItalic(boolean value)](#setItalic-boolean-) | يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يعيّن وقت التعديل الأخير. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | يحصل أو يعيّن تنسيق الرقم المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. |
| [setRestart(int value)](#setRestart-int-) | يحصل أو يعيّن القيمة الرقمية التي تتجاوز القيمة العددية التلقائية لعنصر القائمة. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


ينشئ مثيلاً جديداً لفئة `NumberList`. هذا المثيل يمثل قائمة نقطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | رمز يمثل نقطة. |
| font | java.lang.String | خط للنقطة. |
| fontSize | int | حجم الخط للنقطة. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


ينشئ مثيلاً جديداً لفئة `NumberList`. هذا المثيل يمثل قائمة مرقمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تنسيق | java.lang.String | تنسيق الرأس المرقم. |
| numberFormat | byte | تنسيق الرقم في الرأس. |
| font | java.lang.String | خط للعنوان المرقم. |
| fontSize | int | حجم الخط للعنوان المرقم. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


يحدد ما إذا كان الكائن المحدد يساوي الكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | الكائن. |

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
### getFont() {#getFont--}
```
public String getFont()
```


يحصل أو يعيّن اسم الخط.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


يحصل أو يعيّن لون الخط.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


يحصل أو يضبط حجم الخط.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


يحصل أو يضبط تنسيق رأس السطر. بالنسبة للقوائم النقطية يمثل رمزًا نقطيًا.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل أو يعيّن وقت التعديل الأخير.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


يحصل أو يضبط تنسيق الرقم المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. يجب أن يكون فارغًا للقوائم النقطية.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


يحصل على رأس القائمة المرقمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sequenceNumber | int | رقم التسلسل في القائمة المرقمة. |

**Returns:**
java.lang.String - تمثيل نصي للرقم التسلسلي المحدد.
### getRestart() {#getRestart--}
```
public int getRestart()
```


يحصل أو يعيّن القيمة الرقمية التي تتجاوز القيمة العددية التلقائية لعنصر القائمة.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة للنوع.

**Returns:**
عدد صحيح - ال `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص غامقًا.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص غامقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


يحصل أو يعيّن اسم الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


يحصل أو يعيّن لون الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


يحصل أو يضبط حجم الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


يحصل أو يضبط تنسيق رأس السطر. بالنسبة للقوائم النقطية يمثل رمزًا نقطيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


يحصل أو يضبط قيمة تشير إلى ما إذا كان نمط النص مائلًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يعيّن وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


يحصل أو يضبط تنسيق الرقم المستخدم لمجموعة من الكائنات المرقمة تلقائيًا. يجب أن يكون فارغًا للقوائم النقطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


يحصل أو يعيّن القيمة الرقمية التي تتجاوز القيمة العددية التلقائية لعنصر القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

