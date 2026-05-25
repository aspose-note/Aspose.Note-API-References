---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API Reference"
description: "Allows to specify additional options when rendering document pages to images."
type: docs
weight: 35
url: /hi/java/com.aspose.note/imagesaveoptions/
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
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initializes a new instance of the `ImageSaveOptions` class. |
## Methods

| Method | Description |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | छवि के बाइनराइज़ेशन के विकल्प प्राप्त करता है या सेट करता है। |
| [getColorMode()](#getColorMode--) | प्राप्त करता है या सेट करता है `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) आउटपुट छवि के लिए। |
| [getQuality()](#getQuality--) | सहेजी गई छवि की गुणवत्ता निर्धारित करने वाला मान प्राप्त करता है। |
| [getResolution()](#getResolution--) | जनरेट की गई छवियों के लिए रिज़ॉल्यूशन प्राप्त करता है, डॉट्स प्रति इंच में। |
| [getTiffCompression()](#getTiffCompression--) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | छवि के बाइनराइज़ेशन के विकल्प प्राप्त करता है या सेट करता है। |
| [setColorMode(int value)](#setColorMode-int-) | प्राप्त करता है या सेट करता है `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) आउटपुट छवि के लिए। |
| [setQuality(int value)](#setQuality-int-) | Sets a value determining the quality of saved image. |
| [setResolution(float value)](#setResolution-float-) | Sets the resolution for the generated images, in dots per inch. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Gets or sets the type of compression to use when saving generated images to the TIFF format. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initializes a new instance of the `ImageSaveOptions` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The format in which the document is saved. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


छवि के बाइनराइज़ेशन के विकल्प प्राप्त करता है या सेट करता है।

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


प्राप्त करता है या सेट करता है `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) आउटपुट छवि के लिए।

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


जनरेट की गई छवियों के लिए रिज़ॉल्यूशन प्राप्त करता है, डॉट्स प्रति इंच में।

--------------------

डिफ़ॉल्ट मान 96 है।

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Gets or sets the type of compression to use when saving generated images to the TIFF format.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


छवि के बाइनराइज़ेशन के विकल्प प्राप्त करता है या सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


प्राप्त करता है या सेट करता है `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) आउटपुट छवि के लिए।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


सहेजी गई छवि की गुणवत्ता निर्धारित करने वाला मान सेट करता है। यह मान कोडेक को System.Drawing.Imaging.Encoder.Quality पैरामीटर के रूप में पास किया जाता है।

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

