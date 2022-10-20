---
title: ImageSaveOptions
second_title: Aspose.Note for Java API Reference
description: Allows to specify additional options when rendering document pages to images.
type: docs
weight: 27
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
| [getResolution()](#getResolution--) | Gets the resolution for the generated images, in dots per inch. |
| [setResolution(float value)](#setResolution-float-) | Sets the resolution for the generated images, in dots per inch. |
| [getQuality()](#getQuality--) | Gets a value determining the quality of saved image. |
| [setQuality(int value)](#setQuality-int-) | Sets a value determining the quality of saved image. |
| [getColorMode()](#getColorMode--) | Gets or sets  ColorMode (\#getColorMode.getColorMode/\#setColorMode(int).setColorMode(int)) for the output image. |
| [setColorMode(int value)](#setColorMode-int-) | Gets or sets  ColorMode (\#getColorMode.getColorMode/\#setColorMode(int).setColorMode(int)) for the output image. |
| [getBinarizationOptions()](#getBinarizationOptions--) | Gets or sets options for image's binarization. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Gets or sets options for image's binarization. |
| [getTiffCompression()](#getTiffCompression--) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initializes a new instance of the  ImageSaveOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The format in which the document is saved. |

### getResolution() {#getResolution--}
```
public float getResolution()
```


Gets the resolution for the generated images, in dots per inch.

--------------------

The default value is 96.

**Returns:**
float
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

### getQuality() {#getQuality--}
```
public final int getQuality()
```


Gets a value determining the quality of saved image. This value is passed to codec as System.Drawing.Imaging.Encoder.Quality parameter.

--------------------

The range of useful values for the quality category is from 0 to 100. The lower the number specified, the higher the compression and therefore the lower the quality of the image. Zero would give you the lowest quality image and 100 the highest. The default value is 90.

**Returns:**
int
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

### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Gets or sets  ColorMode (\#getColorMode.getColorMode/\#setColorMode(int).setColorMode(int)) for the output image.

**Returns:**
int
### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Gets or sets  ColorMode (\#getColorMode.getColorMode/\#setColorMode(int).setColorMode(int)) for the output image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Gets or sets options for image's binarization.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Gets or sets options for image's binarization.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Gets or sets the type of compression to use when saving generated images to the TIFF format.

**Returns:**
int
### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Gets or sets the type of compression to use when saving generated images to the TIFF format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

