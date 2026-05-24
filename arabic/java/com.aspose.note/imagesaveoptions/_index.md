---
title: "ImageSaveOptions"
second_title: "مرجع Aspose.Note for Java API"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى صور."
type: docs
weight: 35
url: /ar/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المستند إلى صور.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | ينشئ مثيلًا جديدًا للفئة `ImageSaveOptions`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | يحصل أو يعيّن خيارات ثنائية الصورة. |
| [getColorMode()](#getColorMode--) | يحصل أو يعيّن `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) للصورة الناتجة. |
| [getQuality()](#getQuality--) | يحصل على قيمة تحدد جودة الصورة المحفوظة. |
| [getResolution()](#getResolution--) | يحصل على الدقة للصور المولدة، بوحدة النقاط في البوصة. |
| [getTiffCompression()](#getTiffCompression--) | يحصل أو يعيّن نوع الضغط الذي يُستخدم عند حفظ الصور المُولّدة بتنسيق TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | يحصل أو يعيّن خيارات ثنائية الصورة. |
| [setColorMode(int value)](#setColorMode-int-) | يحصل أو يعيّن `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) للصورة الناتجة. |
| [setQuality(int value)](#setQuality-int-) | يعيّن قيمة تحدد جودة الصورة المحفوظة. |
| [setResolution(float value)](#setResolution-float-) | يعيّن الدقة للصور المُولّدة، بوحدة النقاط في البوصة. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | يحصل أو يعيّن نوع الضغط الذي يُستخدم عند حفظ الصور المُولّدة بتنسيق TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


ينشئ مثيلًا جديدًا للفئة `ImageSaveOptions`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| format | int | التنسيق الذي يُحفظ به المستند. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


يحصل أو يعيّن خيارات ثنائية الصورة.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


يحصل أو يعيّن `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) للصورة الناتجة.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


يحصل على قيمة تحدد جودة الصورة المحفوظة. تُمرّر هذه القيمة إلى برنامج الترميز كمعامل System.Drawing.Imaging.Encoder.Quality.

--------------------

نطاق القيم المفيدة لفئة الجودة هو من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. الصفر يعطيك أدنى جودة للصورة و100 أعلى جودة. القيمة الافتراضية هي 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


يحصل على الدقة للصور المولدة، بوحدة النقاط في البوصة.

--------------------

القيمة الافتراضية هي 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


يحصل أو يعيّن نوع الضغط الذي يُستخدم عند حفظ الصور المُولّدة بتنسيق TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


يحصل أو يعيّن خيارات ثنائية الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


يحصل أو يعيّن `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) للصورة الناتجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


يعيّن قيمة تحدد جودة الصورة المحفوظة. تُمرّر هذه القيمة إلى برنامج الترميز كمعامل System.Drawing.Imaging.Encoder.Quality.

--------------------

نطاق القيم المفيدة لفئة الجودة هو من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. الصفر يعطيك أدنى جودة للصورة و100 أعلى جودة. القيمة الافتراضية هي 90.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


يعيّن الدقة للصور المُولّدة، بوحدة النقاط في البوصة.

--------------------

القيمة الافتراضية هي 90.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


يحصل أو يعيّن نوع الضغط الذي يُستخدم عند حفظ الصور المُولّدة بتنسيق TIFF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

