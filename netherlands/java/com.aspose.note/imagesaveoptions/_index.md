---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Staat toe extra opties op te geven bij het renderen van documentpagina's naar afbeeldingen."
type: docs
weight: 35
url: /nl/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Staat toe extra opties op te geven bij het renderen van documentpagina's naar afbeeldingen.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initialiseert een nieuw exemplaar van de `ImageSaveOptions`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Haalt of stelt opties in voor de binarisatie van de afbeelding. |
| [getColorMode()](#getColorMode--) | Haalt of stelt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) in voor de uitvoerafbeelding. |
| [getQuality()](#getQuality--) | Haalt een waarde op die de kwaliteit van de opgeslagen afbeelding bepaalt. |
| [getResolution()](#getResolution--) | Haalt de resolutie op voor de gegenereerde afbeeldingen, in punten per inch. |
| [getTiffCompression()](#getTiffCompression--) | Haalt op of stelt het type compressie in dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Haalt of stelt opties in voor de binarisatie van de afbeelding. |
| [setColorMode(int value)](#setColorMode-int-) | Haalt of stelt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) in voor de uitvoerafbeelding. |
| [setQuality(int value)](#setQuality-int-) | Stelt een waarde in die de kwaliteit van de opgeslagen afbeelding bepaalt. |
| [setResolution(float value)](#setResolution-float-) | Stelt de resolutie in voor de gegenereerde afbeeldingen, in dots per inch. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Haalt op of stelt het type compressie in dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initialiseert een nieuw exemplaar van de `ImageSaveOptions`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| format | int | Het formaat waarin het document wordt opgeslagen. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Haalt of stelt opties in voor de binarisatie van de afbeelding.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Haalt of stelt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) in voor de uitvoerafbeelding.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Haalt een waarde op die de kwaliteit van de opgeslagen afbeelding bepaalt. Deze waarde wordt doorgegeven aan de codec als de System.Drawing.Imaging.Encoder.Quality‑parameter.

--------------------

Het bereik van bruikbare waarden voor de kwaliteitscategorie is van 0 tot 100. Hoe lager het opgegeven getal, hoe hoger de compressie en dus hoe lager de kwaliteit van de afbeelding. Nul geeft de laagste kwaliteit afbeelding en 100 de hoogste. De standaardwaarde is 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Haalt de resolutie op voor de gegenereerde afbeeldingen, in punten per inch.

--------------------

De standaardwaarde is 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Haalt op of stelt het type compressie in dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Haalt of stelt opties in voor de binarisatie van de afbeelding.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Haalt of stelt `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) in voor de uitvoerafbeelding.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Stelt een waarde in die de kwaliteit van de opgeslagen afbeelding bepaalt. Deze waarde wordt doorgegeven aan de codec als de System.Drawing.Imaging.Encoder.Quality‑parameter.

--------------------

Het bereik van bruikbare waarden voor de kwaliteitscategorie is van 0 tot 100. Hoe lager het opgegeven getal, hoe hoger de compressie en dus hoe lager de kwaliteit van de afbeelding. Nul geeft de laagste kwaliteit afbeelding en 100 de hoogste. De standaardwaarde is 90.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Stelt de resolutie in voor de gegenereerde afbeeldingen, in dots per inch.

--------------------

De standaardwaarde is 90.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Haalt op of stelt het type compressie in dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

