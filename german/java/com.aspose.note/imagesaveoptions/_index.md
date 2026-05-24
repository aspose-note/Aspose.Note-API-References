---
title: "ImageSaveOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Dokumentseiten zu Bildern."
type: docs
weight: 35
url: /de/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Dokumentseiten zu Bildern.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initialisiert eine neue Instanz der Klasse `ImageSaveOptions`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Liest oder setzt Optionen für die Binarisierung des Bildes. |
| [getColorMode()](#getColorMode--) | Liest oder setzt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) für das Ausgabebild. |
| [getQuality()](#getQuality--) | Liest einen Wert, der die Qualität des gespeicherten Bildes bestimmt. |
| [getResolution()](#getResolution--) | Liest die Auflösung der erzeugten Bilder in Punkten pro Zoll. |
| [getTiffCompression()](#getTiffCompression--) | Liest oder legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format verwendet wird. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Liest oder setzt Optionen für die Binarisierung des Bildes. |
| [setColorMode(int value)](#setColorMode-int-) | Liest oder setzt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) für das Ausgabebild. |
| [setQuality(int value)](#setQuality-int-) | Legt einen Wert fest, der die Qualität des gespeicherten Bildes bestimmt. |
| [setResolution(float value)](#setResolution-float-) | Legt die Auflösung für die erzeugten Bilder in Punkten pro Zoll fest. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Liest oder legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format verwendet wird. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initialisiert eine neue Instanz der Klasse `ImageSaveOptions`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | int | Das Format, in dem das Dokument gespeichert wird. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Liest oder setzt Optionen für die Binarisierung des Bildes.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Liest oder setzt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) für das Ausgabebild.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Liest einen Wert, der die Qualität des gespeicherten Bildes bestimmt. Dieser Wert wird dem Codec als Parameter System.Drawing.Imaging.Encoder.Quality übergeben.

--------------------

Der Bereich nützlicher Werte für die Qualitätskategorie liegt zwischen 0 und 100. Je niedriger die angegebene Zahl, desto höher die Kompression und damit desto niedriger die Bildqualität. Null ergibt das Bild mit der niedrigsten Qualität und 100 die höchste. Der Standardwert ist 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Liest die Auflösung der erzeugten Bilder in Punkten pro Zoll.

--------------------

Der Standardwert ist 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Liest oder legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format verwendet wird.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Liest oder setzt Optionen für die Binarisierung des Bildes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Liest oder setzt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) für das Ausgabebild.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Legt einen Wert fest, der die Qualität des gespeicherten Bildes bestimmt. Dieser Wert wird dem Codec als Parameter System.Drawing.Imaging.Encoder.Quality übergeben.

--------------------

Der Bereich nützlicher Werte für die Qualitätskategorie liegt zwischen 0 und 100. Je niedriger die angegebene Zahl, desto höher die Kompression und damit desto niedriger die Bildqualität. Null ergibt das Bild mit der niedrigsten Qualität und 100 die höchste. Der Standardwert ist 90.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Legt die Auflösung für die erzeugten Bilder in Punkten pro Zoll fest.

--------------------

Der Standardwert ist 90.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Liest oder legt den Kompressionstyp fest, der beim Speichern erzeugter Bilder im TIFF-Format verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

