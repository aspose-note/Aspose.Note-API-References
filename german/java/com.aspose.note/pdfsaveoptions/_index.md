---
title: "PdfSaveOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Dokumentseiten zu PDF."
type: docs
weight: 77
url: /de/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Ermöglicht das Angeben zusätzlicher Optionen beim Rendern von Dokumentseiten zu PDF.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Initialisiert eine neue Instanz der `PdfSaveOptions`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Ermittelt den Kompressionstyp, der auf Bilder in der PDF-Datei angewendet wird. |
| [getJpegQuality()](#getJpegQuality--) | Ermittelt einen Wert, der die Qualität der JPEG-Bilder im PDF-Dokument bestimmt. |
| [getPageSettings()](#getPageSettings--) | Liest oder legt die Seiteneinstellungen für jede Seite im Dokument fest. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Liest oder legt den für die Seitenteilung verwendeten Algorithmus fest. |
| [setImageCompression(int value)](#setImageCompression-int-) | Legt den Kompressionstyp fest, der auf Bilder in der PDF-Datei angewendet wird. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Legt einen Wert fest, der die Qualität der JPEG-Bilder im PDF-Dokument bestimmt. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Liest oder legt die Seiteneinstellungen für jede Seite im Dokument fest. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Liest oder legt den für die Seitenteilung verwendeten Algorithmus fest. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Initialisiert eine neue Instanz der `PdfSaveOptions`-Klasse.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Ermittelt den Kompressionstyp, der auf Bilder in der PDF-Datei angewendet wird.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Ermittelt einen Wert, der die Qualität der JPEG-Bilder im PDF-Dokument bestimmt. Der Wert kann von 0 bis 100 variieren, wobei 0 die schlechteste Qualität aber maximale Kompression bedeutet und 100 die beste Qualität aber minimale Kompression.

--------------------

Der Standardwert ist 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Liest oder legt die Seiteneinstellungen für jede Seite im Dokument fest. Standardmäßig hängt es von CurrentUICulture ab, \*US-Kulturen haben das Letter-Format, andere haben das A4-Format.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Liest oder legt den für die Seitenteilung verwendeten Algorithmus fest.

Wert: Der `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Legt den Kompressionstyp fest, der auf Bilder in der PDF-Datei angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Legt einen Wert fest, der die Qualität der JPEG-Bilder im PDF-Dokument bestimmt. Der Wert kann von 0 bis 100 variieren, wobei 0 die schlechteste Qualität aber maximale Kompression bedeutet und 100 die beste Qualität aber minimale Kompression.

--------------------

Der Standardwert ist 90.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Liest oder legt die Seiteneinstellungen für jede Seite im Dokument fest. Standardmäßig hängt es von CurrentUICulture ab, \*US-Kulturen haben das Letter-Format, andere haben das A4-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Liest oder legt den für die Seitenteilung verwendeten Algorithmus fest.

Wert: Der `PageSplittingAlgorithm`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

