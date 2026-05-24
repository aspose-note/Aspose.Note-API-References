---
title: "PdfSaveOptions"
second_title: "مرجع Aspose.Note for Java API"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى PDF."
type: docs
weight: 77
url: /ar/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى PDF.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | يُنشئ مثيلاً جديدًا من الفئة `PdfSaveOptions`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | يحصل على نوع الضغط المطبق على الصور في ملف PDF. |
| [getJpegQuality()](#getJpegQuality--) | يحصل على قيمة تحدد جودة صور JPEG داخل مستند PDF. |
| [getPageSettings()](#getPageSettings--) | يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات. |
| [setImageCompression(int value)](#setImageCompression-int-) | يضبط نوع الضغط المطبق على الصور في ملف PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | يضبط قيمة تحدد جودة صور JPEG داخل مستند PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


يُنشئ مثيلاً جديدًا من الفئة `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


يحصل على نوع الضغط المطبق على الصور في ملف PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


يحصل على قيمة تحدد جودة صور JPEG داخل مستند PDF. قد تتراوح القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة ولكن أقصى ضغط و100 يعني أفضل جودة ولكن أقل ضغط.

--------------------

القيمة الافتراضية هي 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture، \*US الثقافات لديها إعداد letter، الأخرى لديها إعداد A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات.

القيمة: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


يضبط نوع الضغط المطبق على الصور في ملف PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


يضبط قيمة تحدد جودة صور JPEG داخل مستند PDF. قد تتراوح القيمة من 0 إلى 100 حيث يعني 0 أسوأ جودة ولكن أقصى ضغط و100 يعني أفضل جودة ولكن أقل ضغط.

--------------------

القيمة الافتراضية هي 90.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


يحصل أو يضبط إعدادات الصفحة لكل صفحة في المستند. بشكل افتراضي يعتمد على CurrentUICulture، \*US الثقافات لديها إعداد letter، الأخرى لديها إعداد A4.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


يحصل أو يضبط الخوارزمية المستخدمة لتقسيم الصفحات.

القيمة: `PageSplittingAlgorithm`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

