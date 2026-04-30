---
title: PdfSaveOptions
second_title: Aspose.Note for Java API Reference
description: Allows to specify additional options when rendering document pages to PDF.
type: docs
weight: 77
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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontsSubsystem()](#getFontsSubsystem--) | Gets or sets font's settings to be used while saving |
| [getImageCompression()](#getImageCompression--) | Gets the type of compression applied to images in the PDF file. |
| [getJpegQuality()](#getJpegQuality--) | Gets a value determining the quality of the JPEG images inside PDF document. |
| [getPageCount()](#getPageCount--) | Gets or sets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets or sets the index of the first page to save. |
| [getPageSettings()](#getPageSettings--) | Gets or sets the page settings for each page in document. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Gets or sets algorithm used for page splitting. |
| [getSaveFormat()](#getSaveFormat--) | Gets or sets the format in which the document is saved. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Gets or sets font's settings to be used while saving |
| [setImageCompression(int value)](#setImageCompression-int-) | Sets the type of compression applied to images in the PDF file. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Sets a value determining the quality of the JPEG images inside PDF document. |
| [setPageCount(int value)](#setPageCount-int-) | Gets or sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Gets or sets the index of the first page to save. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Gets or sets the page settings for each page in document. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Gets or sets algorithm used for page splitting. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initializes a new instance of the  PdfSaveOptions  class.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Gets or sets font's settings to be used while saving

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Gets the type of compression applied to images in the PDF file.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Gets a value determining the quality of the JPEG images inside PDF document. The value may vary from 0 to 100 where 0 means worst quality but maximum compression and 100 means best quality but minimum compression.

--------------------

The default value is 90.

**Returns:**
int
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gets or sets the number of pages to save. By default is \{@link int\#Int32Extensions.MaxValue\} which means all pages of the document will be rendered.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Gets or sets the index of the first page to save. By default is 0.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Gets or sets the page settings for each page in document. By default depends on CurrentUICulture, \*US cultures have letter setting, other have A4 settings.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Gets or sets algorithm used for page splitting.

Value: The  PageSplittingAlgorithm .

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets or sets the format in which the document is saved.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Gets or sets font's settings to be used while saving

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Sets the type of compression applied to images in the PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Gets or sets the number of pages to save. By default is \{@link int\#Int32Extensions.MaxValue\} which means all pages of the document will be rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Gets or sets the index of the first page to save. By default is 0.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Gets or sets the page settings for each page in document. By default depends on CurrentUICulture, \*US cultures have letter setting, other have A4 settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

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

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

