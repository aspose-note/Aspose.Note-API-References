---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API 参考"
description: "允许在将文档页面渲染为图像时指定其他选项。"
type: docs
weight: 35
url: /zh/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

允许在将文档页面渲染为图像时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | 初始化 `ImageSaveOptions` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | 获取或设置图像二值化的选项。 |
| [getColorMode()](#getColorMode--) | 获取或设置输出图像的 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))。 |
| [getQuality()](#getQuality--) | 获取决定已保存图像质量的值。 |
| [getResolution()](#getResolution--) | 获取生成图像的分辨率（每英寸点数）。 |
| [getTiffCompression()](#getTiffCompression--) | 获取或设置在将生成的图像保存为 TIFF 格式时使用的压缩类型。 |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | 获取或设置图像二值化的选项。 |
| [setColorMode(int value)](#setColorMode-int-) | 获取或设置输出图像的 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))。 |
| [setQuality(int value)](#setQuality-int-) | 设置决定已保存图像质量的值。 |
| [setResolution(float value)](#setResolution-float-) | 设置生成图像的分辨率（每英寸点数）。 |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 获取或设置在将生成的图像保存为 TIFF 格式时使用的压缩类型。 |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


初始化 `ImageSaveOptions` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | int | 文档保存的格式。 |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


获取或设置图像二值化的选项。

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


获取或设置输出图像的 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))。

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


获取决定已保存图像质量的值。该值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器。

--------------------

质量类别的有效值范围为 0 到 100。指定的数值越低，压缩率越高，图像质量越低。0 将产生最低质量的图像，100 则为最高质量。默认值为 90。

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


获取生成图像的分辨率（每英寸点数）。

--------------------

默认值为 96。

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


获取或设置在将生成的图像保存为 TIFF 格式时使用的压缩类型。

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


获取或设置图像二值化的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


获取或设置输出图像的 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


设置决定已保存图像质量的值。该值作为 System.Drawing.Imaging.Encoder.Quality 参数传递给编解码器。

--------------------

质量类别的有效值范围为 0 到 100。指定的数值越低，压缩率越高，图像质量越低。0 将产生最低质量的图像，100 则为最高质量。默认值为 90。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


设置生成图像的分辨率（每英寸点数）。

--------------------

默认值为 90。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


获取或设置在将生成的图像保存为 TIFF 格式时使用的压缩类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

