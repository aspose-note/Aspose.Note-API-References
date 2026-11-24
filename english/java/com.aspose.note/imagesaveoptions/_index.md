---
title: ImageSaveOptions
second_title: Aspose.Note for Java API Reference
description: Allows to specify additional options when rendering document pages to images.
type: docs
weight: 35
url: /java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Allows to specify additional options when rendering document pages to images.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initializes a new instance of the  ImageSaveOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinarizationOptions()](#getBinarizationOptions--) | Gets or sets options for image's binarization. |
| [getClass()](#getClass--) |  |
| [getColorMode()](#getColorMode--) | Gets or sets  ColorMode ([.getColorMode](../../null/\#getColorMode)/[.setColorMode(int)](../../null/\#setColorMode-int-)) for the output image. |
| [getFontsSubsystem()](#getFontsSubsystem--) | Gets or sets font's settings to be used while saving |
| [getPageCount()](#getPageCount--) | Gets or sets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets or sets the index of the first page to save. |
| [getQuality()](#getQuality--) | Gets a value determining the quality of saved image. |
| [getResolution()](#getResolution--) | Gets the resolution for the generated images, in dots per inch. |
| [getSaveFormat()](#getSaveFormat--) | Gets or sets the format in which the document is saved. |
| [getTiffCompression()](#getTiffCompression--) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Gets or sets options for image's binarization. |
| [setColorMode(int value)](#setColorMode-int-) | Gets or sets  ColorMode ([.getColorMode](../../null/\#getColorMode)/[.setColorMode(int)](../../null/\#setColorMode-int-)) for the output image. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Gets or sets font's settings to be used while saving |
| [setPageCount(int value)](#setPageCount-int-) | Gets or sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Gets or sets the index of the first page to save. |
| [setQuality(int value)](#setQuality-int-) | Sets a value determining the quality of saved image. |
| [setResolution(float value)](#setResolution-float-) | Sets the resolution for the generated images, in dots per inch. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initializes a new instance of the  ImageSaveOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The format in which the document is saved. |

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
### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Gets or sets options for image's binarization.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Gets or sets  ColorMode ([.getColorMode](../../null/\#getColorMode)/[.setColorMode(int)](../../null/\#setColorMode-int-)) for the output image.

**Returns:**
int
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Gets or sets font's settings to be used while saving

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
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
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Gets a value determining the quality of saved image. This value is passed to codec as System.Drawing.Imaging.Encoder.Quality parameter.

--------------------

The range of useful values for the quality category is from 0 to 100. The lower the number specified, the higher the compression and therefore the lower the quality of the image. Zero would give you the lowest quality image and 100 the highest. The default value is 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Gets the resolution for the generated images, in dots per inch.

--------------------

The default value is 96.

**Returns:**
float
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets or sets the format in which the document is saved.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Gets or sets the type of compression to use when saving generated images to the TIFF format.

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




### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Gets or sets options for image's binarization.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Gets or sets  ColorMode ([.getColorMode](../../null/\#getColorMode)/[.setColorMode(int)](../../null/\#setColorMode-int-)) for the output image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Gets or sets font's settings to be used while saving

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

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

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Sets a value determining the quality of saved image. This value is passed to codec as System.Drawing.Imaging.Encoder.Quality parameter.

--------------------

The range of useful values for the quality category is from 0 to 100. The lower the number specified, the higher the compression and therefore the lower the quality of the image. Zero would give you the lowest quality image and 100 the highest. The default value is 90.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Sets the resolution for the generated images, in dots per inch.

--------------------

The default value is 90.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Gets or sets the type of compression to use when saving generated images to the TIFF format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

