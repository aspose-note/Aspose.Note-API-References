---
title: "PdfSaveOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Staat toe extra opties op te geven bij het renderen van documentpagina's naar PDF."
type: docs
weight: 77
url: /nl/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Staat toe extra opties op te geven bij het renderen van documentpagina's naar PDF.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialiseert een nieuw exemplaar van de `PdfSaveOptions` klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Haalt het type compressie op dat wordt toegepast op afbeeldingen in het PDF‑bestand. |
| [getJpegQuality()](#getJpegQuality--) | Haalt een waarde op die de kwaliteit van de JPEG‑afbeeldingen in het PDF‑document bepaalt. |
| [getPageSettings()](#getPageSettings--) | Haalt op of stelt de pagina-instellingen in voor elke pagina in het document. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Haalt op of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's. |
| [setImageCompression(int value)](#setImageCompression-int-) | Stelt het type compressie in dat wordt toegepast op afbeeldingen in het PDF‑bestand. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Stelt een waarde in die de kwaliteit van de JPEG‑afbeeldingen in het PDF‑document bepaalt. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Haalt op of stelt de pagina-instellingen in voor elke pagina in het document. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Haalt op of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialiseert een nieuw exemplaar van de `PdfSaveOptions` klasse.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Haalt het type compressie op dat wordt toegepast op afbeeldingen in het PDF‑bestand.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Haalt een waarde op die de kwaliteit van de JPEG‑afbeeldingen in het PDF‑document bepaalt. De waarde kan variëren van 0 tot 100, waarbij 0 de slechtste kwaliteit maar maximale compressie betekent en 100 de beste kwaliteit maar minimale compressie.

--------------------

De standaardwaarde is 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Haalt op of stelt de pagina-instellingen in voor elke pagina in het document. Standaard hangt dit af van CurrentUICulture, \*US-culturen hebben de letter‑instelling, andere hebben A4‑instellingen.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Haalt op of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's.

Waarde: De `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Stelt het type compressie in dat wordt toegepast op afbeeldingen in het PDF‑bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Stelt een waarde in die de kwaliteit van de JPEG‑afbeeldingen in het PDF‑document bepaalt. De waarde kan variëren van 0 tot 100, waarbij 0 de slechtste kwaliteit maar maximale compressie betekent en 100 de beste kwaliteit maar minimale compressie.

--------------------

De standaardwaarde is 90.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Haalt op of stelt de pagina-instellingen in voor elke pagina in het document. Standaard hangt dit af van CurrentUICulture, \*US-culturen hebben de letter‑instelling, andere hebben A4‑instellingen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Haalt op of stelt het algoritme in dat wordt gebruikt voor het splitsen van pagina's.

Waarde: De `PageSplittingAlgorithm`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

