---
title: "DocumentPrintAttributeSet"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل فئة مساعدة بواجهة سهلة الاستخدام مع AttributeSet."
type: docs
weight: 21
url: /ar/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

يمثل فئة مساعدة بواجهة سهلة الاستخدام مع AttributeSet.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | يضبط قيمة تشير إلى ما إذا كان المستند مُرتّبًا. |
| [setCopies(int value)](#setCopies-int-) | يضبط عدد النسخ التي سيتم طباعتها. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | يضبط إعداد الطابعة للطباعة على الوجهين. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | يضبط اتجاه الصفحة. |
| [setPrintRange(int page)](#setPrintRange-int-) | يضبط الصفحة الفردية التي سيتم طباعتها. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | يضبط نطاق الصفحات التي سيتم طباعتها. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | اسم الطابعة التي سيتم استخدامها. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | اسم الطابعة التي سيتم استخدامها. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. بشكل افتراضي تُطبع جميع صفحات المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نسخ | int | عدد نسخ المستند التي سيتم طباعتها. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. بشكل افتراضي تُطبع جميع صفحات المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة. |
| نسخ | int | عدد نسخ المستند التي سيتم طباعتها. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. بشكل افتراضي النسخة الوحيدة لكل صفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


ينشئ مثيلًا جديدًا من `DocumentPrintAttributeSet`. بشكل افتراضي النسخة الوحيدة لكل صفحة.

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان المستند مُرتّبًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | `true` يعادل إعداد SheetCollate.COLLATED `false` يعادل إعداد SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


يضبط عدد النسخ التي سيتم طباعتها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد النسخ التي سيتم طباعتها. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


يضبط إعداد الطابعة للطباعة على الوجهين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | `true` يعادل إعداد Sides.DUPLEX `false` يعادل إعداد Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


يضبط اتجاه الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | `true` يعادل إعداد OrientationRequested.LANDSCAPE `false` يعادل إعداد OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


يضبط الصفحة الفردية التي سيتم طباعتها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صفحة | int | الصفحة التي سيتم طباعتها. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


يضبط نطاق الصفحات التي سيتم طباعتها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| من | int | الصفحة الأولى. |
| إلى | int | الصفحة الأخيرة. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


اسم الطابعة التي سيتم استخدامها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


اسم الطابعة التي سيتم استخدامها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| printerName | java.lang.String | اسم الطابعة. |
| locale | java.util.Locale | اللغة الخاصة بـ printerName. |

