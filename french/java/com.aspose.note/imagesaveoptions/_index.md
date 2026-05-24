---
title: "ImageSaveOptions"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages du document en images."
type: docs
weight: 35
url: /fr/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages du document en images.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Initialise une nouvelle instance de la classe `ImageSaveOptions`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Obtient ou définit les options de binarisation de l'image. |
| [getColorMode()](#getColorMode--) | Obtient ou définit `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) pour l'image de sortie. |
| [getQuality()](#getQuality--) | Obtient une valeur déterminant la qualité de l'image enregistrée. |
| [getResolution()](#getResolution--) | Obtient la résolution des images générées, en points par pouce. |
| [getTiffCompression()](#getTiffCompression--) | Obtient ou définit le type de compression à utiliser lors de l'enregistrement des images générées au format TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Obtient ou définit les options de binarisation de l'image. |
| [setColorMode(int value)](#setColorMode-int-) | Obtient ou définit `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) pour l'image de sortie. |
| [setQuality(int value)](#setQuality-int-) | Définit une valeur déterminant la qualité de l'image enregistrée. |
| [setResolution(float value)](#setResolution-float-) | Définit la résolution des images générées, en points par pouce. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Obtient ou définit le type de compression à utiliser lors de l'enregistrement des images générées au format TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Initialise une nouvelle instance de la classe `ImageSaveOptions`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| format | int | Le format dans lequel le document est enregistré. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Obtient ou définit les options de binarisation de l'image.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Obtient ou définit `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) pour l'image de sortie.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Obtient une valeur déterminant la qualité de l'image enregistrée. Cette valeur est transmise au codec comme paramètre System.Drawing.Imaging.Encoder.Quality.

--------------------

La plage de valeurs utiles pour la catégorie de qualité va de 0 à 100. Plus le nombre spécifié est bas, plus la compression est élevée et donc la qualité de l'image est moindre. Zéro donne l'image de la plus basse qualité et 100 la plus haute. La valeur par défaut est 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Obtient la résolution des images générées, en points par pouce.

--------------------

La valeur par défaut est 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Obtient ou définit le type de compression à utiliser lors de l'enregistrement des images générées au format TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Obtient ou définit les options de binarisation de l'image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Obtient ou définit `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) pour l'image de sortie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Définit une valeur déterminant la qualité de l'image enregistrée. Cette valeur est transmise au codec comme paramètre System.Drawing.Imaging.Encoder.Quality.

--------------------

La plage de valeurs utiles pour la catégorie de qualité va de 0 à 100. Plus le nombre spécifié est bas, plus la compression est élevée et donc la qualité de l'image est moindre. Zéro donne l'image de la plus basse qualité et 100 la plus haute. La valeur par défaut est 90.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Définit la résolution des images générées, en points par pouce.

--------------------

La valeur par défaut est 90.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Obtient ou définit le type de compression à utiliser lors de l'enregistrement des images générées au format TIFF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

