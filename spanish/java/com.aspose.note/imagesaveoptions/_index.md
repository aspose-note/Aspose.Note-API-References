---
title: "ImageSaveOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Permite especificar opciones adicionales al renderizar páginas del documento a imágenes."
type: docs
weight: 35
url: /es/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Permite especificar opciones adicionales al renderizar páginas del documento a imágenes.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Inicializa una nueva instancia de la clase `ImageSaveOptions`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Obtiene o establece opciones para la binarización de la imagen. |
| [getColorMode()](#getColorMode--) | Obtiene o establece `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) para la imagen de salida. |
| [getQuality()](#getQuality--) | Obtiene un valor que determina la calidad de la imagen guardada. |
| [getResolution()](#getResolution--) | Obtiene la resolución de las imágenes generadas, en puntos por pulgada. |
| [getTiffCompression()](#getTiffCompression--) | Obtiene o establece el tipo de compresión que se usa al guardar imágenes generadas en formato TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Obtiene o establece opciones para la binarización de la imagen. |
| [setColorMode(int value)](#setColorMode-int-) | Obtiene o establece `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) para la imagen de salida. |
| [setQuality(int value)](#setQuality-int-) | Establece un valor que determina la calidad de la imagen guardada. |
| [setResolution(float value)](#setResolution-float-) | Establece la resolución de las imágenes generadas, en puntos por pulgada. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Obtiene o establece el tipo de compresión que se usa al guardar imágenes generadas en formato TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Inicializa una nueva instancia de la clase `ImageSaveOptions`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| format | int | El formato en el que se guarda el documento. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Obtiene o establece opciones para la binarización de la imagen.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Obtiene o establece `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) para la imagen de salida.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Obtiene un valor que determina la calidad de la imagen guardada. Este valor se pasa al códec como parámetro System.Drawing.Imaging.Encoder.Quality.

--------------------

El rango de valores útiles para la categoría de calidad es de 0 a 100. Cuanto menor sea el número especificado, mayor será la compresión y, por lo tanto, menor la calidad de la imagen. Cero le dará la imagen de menor calidad y 100 la de mayor calidad. El valor predeterminado es 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Obtiene la resolución de las imágenes generadas, en puntos por pulgada.

--------------------

El valor predeterminado es 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Obtiene o establece el tipo de compresión que se usa al guardar imágenes generadas en formato TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Obtiene o establece opciones para la binarización de la imagen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Obtiene o establece `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) para la imagen de salida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Establece un valor que determina la calidad de la imagen guardada. Este valor se pasa al códec como parámetro System.Drawing.Imaging.Encoder.Quality.

--------------------

El rango de valores útiles para la categoría de calidad es de 0 a 100. Cuanto menor sea el número especificado, mayor será la compresión y, por lo tanto, menor la calidad de la imagen. Cero le dará la imagen de menor calidad y 100 la de mayor calidad. El valor predeterminado es 90.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Establece la resolución de las imágenes generadas, en puntos por pulgada.

--------------------

El valor predeterminado es 90.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Obtiene o establece el tipo de compresión que se usa al guardar imágenes generadas en formato TIFF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

