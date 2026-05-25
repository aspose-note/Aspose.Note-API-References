---
title: "ImageSaveOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in immagini."
type: docs
weight: 35
url: /it/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in immagini.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Inizializza una nuova istanza della classe `ImageSaveOptions`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Ottiene o imposta le opzioni per la binarizzazione dell'immagine. |
| [getColorMode()](#getColorMode--) | Ottiene o imposta `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) per l'immagine di output. |
| [getQuality()](#getQuality--) | Ottiene un valore che determina la qualità dell'immagine salvata. |
| [getResolution()](#getResolution--) | Ottiene la risoluzione per le immagini generate, in punti per pollice. |
| [getTiffCompression()](#getTiffCompression--) | Ottiene o imposta il tipo di compressione da utilizzare durante il salvataggio delle immagini generate nel formato TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Ottiene o imposta le opzioni per la binarizzazione dell'immagine. |
| [setColorMode(int value)](#setColorMode-int-) | Ottiene o imposta `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) per l'immagine di output. |
| [setQuality(int value)](#setQuality-int-) | Imposta un valore che determina la qualità dell'immagine salvata. |
| [setResolution(float value)](#setResolution-float-) | Imposta la risoluzione per le immagini generate, in punti per pollice. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Ottiene o imposta il tipo di compressione da utilizzare durante il salvataggio delle immagini generate nel formato TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Inizializza una nuova istanza della classe `ImageSaveOptions`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| format | int | Il formato in cui il documento viene salvato. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Ottiene o imposta le opzioni per la binarizzazione dell'immagine.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Ottiene o imposta `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) per l'immagine di output.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Ottiene un valore che determina la qualità dell'immagine salvata. Questo valore viene passato al codec come parametro System.Drawing.Imaging.Encoder.Quality.

--------------------

L'intervallo di valori utili per la categoria di qualità è da 0 a 100. Più basso è il numero specificato, maggiore è la compressione e quindi più bassa è la qualità dell'immagine. Zero fornisce l'immagine di qualità più bassa e 100 la più alta. Il valore predefinito è 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Ottiene la risoluzione per le immagini generate, in punti per pollice.

--------------------

Il valore predefinito è 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Ottiene o imposta il tipo di compressione da utilizzare durante il salvataggio delle immagini generate nel formato TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Ottiene o imposta le opzioni per la binarizzazione dell'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Ottiene o imposta `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) per l'immagine di output.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Imposta un valore che determina la qualità dell'immagine salvata. Questo valore viene passato al codec come parametro System.Drawing.Imaging.Encoder.Quality.

--------------------

L'intervallo di valori utili per la categoria di qualità è da 0 a 100. Più basso è il numero specificato, maggiore è la compressione e quindi più bassa è la qualità dell'immagine. Zero fornisce l'immagine di qualità più bassa e 100 la più alta. Il valore predefinito è 90.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Imposta la risoluzione per le immagini generate, in punti per pollice.

--------------------

Il valore predefinito è 90.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Ottiene o imposta il tipo di compressione da utilizzare durante il salvataggio delle immagini generate nel formato TIFF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

