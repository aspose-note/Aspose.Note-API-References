---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när dokumentets sidor renderas till bilder."
type: docs
weight: 35
url: /sv/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Tillåter att ange ytterligare alternativ när dokumentets sidor renderas till bilder.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initierar en ny instans av klassen `ImageSaveOptions`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Hämtar eller anger alternativ för bildens binarisering. |
| [getColorMode()](#getColorMode--) | Hämtar eller anger `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) för utdata-bilden. |
| [getQuality()](#getQuality--) | Hämtar ett värde som bestämmer kvaliteten på den sparade bilden. |
| [getResolution()](#getResolution--) | Hämtar upplösningen för de genererade bilderna, i punkter per tum. |
| [getTiffCompression()](#getTiffCompression--) | Hämtar eller anger komprimeringstypen som ska användas när genererade bilder sparas i TIFF-formatet. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Hämtar eller anger alternativ för bildens binarisering. |
| [setColorMode(int value)](#setColorMode-int-) | Hämtar eller anger `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) för utdata-bilden. |
| [setQuality(int value)](#setQuality-int-) | Anger ett värde som bestämmer kvaliteten på den sparade bilden. |
| [setResolution(float value)](#setResolution-float-) | Anger upplösningen för de genererade bilderna, i punkter per tum. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Hämtar eller anger komprimeringstypen som ska användas när genererade bilder sparas i TIFF-formatet. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initierar en ny instans av klassen `ImageSaveOptions`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | int | Formatet som dokumentet sparas i. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Hämtar eller anger alternativ för bildens binarisering.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Hämtar eller anger `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) för utdata-bilden.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Hämtar ett värde som bestämmer kvaliteten på den sparade bilden. Detta värde skickas till codec som parametern System.Drawing.Imaging.Encoder.Quality.

--------------------

Det användbara värdeintervallet för kvalitetskategorin är från 0 till 100. Ju lägre tal som anges, desto högre kompression och därmed lägre bildkvalitet. Noll ger den lägsta bildkvaliteten och 100 den högsta. Standardvärdet är 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Hämtar upplösningen för de genererade bilderna, i punkter per tum.

--------------------

Standardvärdet är 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Hämtar eller anger komprimeringstypen som ska användas när genererade bilder sparas i TIFF-formatet.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Hämtar eller anger alternativ för bildens binarisering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Hämtar eller anger `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) för utdata-bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Anger ett värde som bestämmer kvaliteten på den sparade bilden. Detta värde skickas till codec som parametern System.Drawing.Imaging.Encoder.Quality.

--------------------

Det användbara värdeintervallet för kvalitetskategorin är från 0 till 100. Ju lägre tal som anges, desto högre kompression och därmed lägre bildkvalitet. Noll ger den lägsta bildkvaliteten och 100 den högsta. Standardvärdet är 90.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Anger upplösningen för de genererade bilderna, i punkter per tum.

--------------------

Standardvärdet är 90.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Hämtar eller anger komprimeringstypen som ska användas när genererade bilder sparas i TIFF-formatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

