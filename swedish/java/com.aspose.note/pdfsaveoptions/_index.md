---
title: "PdfSaveOptions"
second_title: "Aspose.Note for Java API-referens"
description: "Tillåter att ange ytterligare alternativ när dokumentets sidor renderas till PDF."
type: docs
weight: 77
url: /sv/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Tillåter att ange ytterligare alternativ när dokumentets sidor renderas till PDF.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initierar en ny instans av klassen `PdfSaveOptions`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Hämtar typen av kompression som tillämpas på bilder i PDF-filen. |
| [getJpegQuality()](#getJpegQuality--) | Hämtar ett värde som bestämmer kvaliteten på JPEG-bilderna i PDF-dokumentet. |
| [getPageSettings()](#getPageSettings--) | Hämtar eller anger sidinställningarna för varje sida i dokumentet. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Hämtar eller anger algoritmen som används för sidindelning. |
| [setImageCompression(int value)](#setImageCompression-int-) | Anger typen av kompression som tillämpas på bilder i PDF-filen. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Anger ett värde som bestämmer kvaliteten på JPEG-bilderna i PDF-dokumentet. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Hämtar eller anger sidinställningarna för varje sida i dokumentet. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Hämtar eller anger algoritmen som används för sidindelning. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initierar en ny instans av klassen `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Hämtar typen av kompression som tillämpas på bilder i PDF-filen.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Hämtar ett värde som bestämmer kvaliteten på JPEG-bilderna i PDF-dokumentet. Värdet kan variera från 0 till 100 där 0 betyder sämst kvalitet men maximal kompression och 100 betyder bästa kvalitet men minimal kompression.

--------------------

Standardvärdet är 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Hämtar eller anger sidinställningarna för varje sida i dokumentet. Som standard beror det på CurrentUICulture, \*US-kulturer har letter-inställning, andra har A4-inställning.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Hämtar eller anger algoritmen som används för sidindelning.

Värde: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Anger typen av kompression som tillämpas på bilder i PDF-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Anger ett värde som bestämmer kvaliteten på JPEG-bilderna i PDF-dokumentet. Värdet kan variera från 0 till 100 där 0 betyder sämst kvalitet men maximal kompression och 100 betyder bästa kvalitet men minimal kompression.

--------------------

Standardvärdet är 90.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Hämtar eller anger sidinställningarna för varje sida i dokumentet. Som standard beror det på CurrentUICulture, \*US-kulturer har letter-inställning, andra har A4-inställning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Hämtar eller anger algoritmen som används för sidindelning.

Värde: `PageSplittingAlgorithm`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

