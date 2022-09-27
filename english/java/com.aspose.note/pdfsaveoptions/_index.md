---
title: PdfSaveOptions
second_title: Aspose.Note for Java API Reference
description: Allows to specify additional options when rendering document pages to PDF.
type: docs
weight: 62
url: /java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Allows to specify additional options when rendering document pages to PDF.
## Constructors

| Constructor | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initializes a new instance of the  PdfSaveOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Gets the type of compression applied to images in the PDF file. |
| [setImageCompression(int value)](#setImageCompression-int-) | Sets the type of compression applied to images in the PDF file. |
| [getJpegQuality()](#getJpegQuality--) | Gets a value determining the quality of the JPEG images inside PDF document. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Sets a value determining the quality of the JPEG images inside PDF document. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Gets or sets algorithm used for page splitting. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Gets or sets algorithm used for page splitting. |
| [getPageSettings()](#getPageSettings--) | Gets or sets the page settings for each page in document. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Gets or sets the page settings for each page in document. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initializes a new instance of the  PdfSaveOptions  class.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Gets the type of compression applied to images in the PDF file.

**Returns:**
int
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Sets the type of compression applied to images in the PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Gets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression.

--------------------

The default value is 90.

**Returns:**
int
### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Sets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression.

--------------------

The default value is 90.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Gets or sets algorithm used for page splitting.

Value: The  PageSplittingAlgorithm .

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Gets or sets algorithm used for page splitting.

Value: The  PageSplittingAlgorithm .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Gets or sets the page settings for each page in document. By default depends on CurrentUICulture, \*US cultures have letter setting, other have A4 settings.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Gets or sets the page settings for each page in document. By default depends on CurrentUICulture, \*US cultures have letter setting, other have A4 settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

