---
title: "ImageSaveOptions"
second_title: "Справочник API Aspose.Note for Java"
description: "Позволяет указать дополнительные параметры при рендеринге страниц документа в изображения."
type: docs
weight: 35
url: /ru/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Позволяет указать дополнительные параметры при рендеринге страниц документа в изображения.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Инициализирует новый экземпляр класса `ImageSaveOptions`. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Получает или задает параметры бинаризации изображения. |
| [getColorMode()](#getColorMode--) | Получает или задает `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) для выходного изображения. |
| [getQuality()](#getQuality--) | Получает значение, определяющее качество сохранённого изображения. |
| [getResolution()](#getResolution--) | Получает разрешение сгенерированных изображений в точках на дюйм. |
| [getTiffCompression()](#getTiffCompression--) | Получает или задает тип сжатия, используемый при сохранении сгенерированных изображений в формате TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Получает или задает параметры бинаризации изображения. |
| [setColorMode(int value)](#setColorMode-int-) | Получает или задает `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) для выходного изображения. |
| [setQuality(int value)](#setQuality-int-) | Устанавливает значение, определяющее качество сохраняемого изображения. |
| [setResolution(float value)](#setResolution-float-) | Устанавливает разрешение сгенерированных изображений в точках на дюйм. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Получает или задает тип сжатия, используемый при сохранении сгенерированных изображений в формате TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Инициализирует новый экземпляр класса `ImageSaveOptions`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| format | int | Формат, в котором сохраняется документ. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Получает или задает параметры бинаризации изображения.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Получает или задает `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) для выходного изображения.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Получает значение, определяющее качество сохраняемого изображения. Это значение передаётся кодеку как параметр System.Drawing.Imaging.Encoder.Quality.

--------------------

Диапазон полезных значений для категории качества от 0 до 100. Чем ниже указанное число, тем выше степень сжатия и, соответственно, ниже качество изображения. Ноль даст изображение самого низкого качества, а 100 — самого высокого. Значение по умолчанию равно 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Получает разрешение сгенерированных изображений в точках на дюйм.

--------------------

Значение по умолчанию равно 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Получает или задает тип сжатия, используемый при сохранении сгенерированных изображений в формате TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Получает или задает параметры бинаризации изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Получает или задает `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) для выходного изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Устанавливает значение, определяющее качество сохраняемого изображения. Это значение передаётся кодеку как параметр System.Drawing.Imaging.Encoder.Quality.

--------------------

Диапазон полезных значений для категории качества от 0 до 100. Чем ниже указанное число, тем выше степень сжатия и, соответственно, ниже качество изображения. Ноль даст изображение самого низкого качества, а 100 — самого высокого. Значение по умолчанию равно 90.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Устанавливает разрешение сгенерированных изображений в точках на дюйм.

--------------------

Значение по умолчанию — 90.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Получает или задает тип сжатия, используемый при сохранении сгенерированных изображений в формате TIFF.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

