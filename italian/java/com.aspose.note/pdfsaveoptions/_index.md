---
title: "PdfSaveOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in PDF."
type: docs
weight: 77
url: /it/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del documento in PDF.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Inizializza una nuova istanza della classe `PdfSaveOptions`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Ottiene il tipo di compressione applicata alle immagini nel file PDF. |
| [getJpegQuality()](#getJpegQuality--) | Ottiene un valore che determina la qualità delle immagini JPEG all'interno del documento PDF. |
| [getPageSettings()](#getPageSettings--) | Ottiene o imposta le impostazioni della pagina per ogni pagina nel documento. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Ottiene o imposta l'algoritmo utilizzato per la divisione delle pagine. |
| [setImageCompression(int value)](#setImageCompression-int-) | Imposta il tipo di compressione applicata alle immagini nel file PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Imposta un valore che determina la qualità delle immagini JPEG all'interno del documento PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Ottiene o imposta le impostazioni della pagina per ogni pagina nel documento. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Ottiene o imposta l'algoritmo utilizzato per la divisione delle pagine. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Inizializza una nuova istanza della classe `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Ottiene il tipo di compressione applicata alle immagini nel file PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Ottiene un valore che determina la qualità delle immagini JPEG all'interno del documento PDF. Il valore può variare da 0 a 100 dove 0 indica la qualità più bassa ma la massima compressione e 100 indica la migliore qualità ma la compressione minima.

--------------------

Il valore predefinito è 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Ottiene o imposta le impostazioni della pagina per ogni pagina nel documento. Per impostazione predefinita dipende da CurrentUICulture, \*US cultures hanno impostazione letter, le altre hanno impostazione A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Ottiene o imposta l'algoritmo utilizzato per la divisione delle pagine.

Valore: Il `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Imposta il tipo di compressione applicata alle immagini nel file PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Imposta un valore che determina la qualità delle immagini JPEG all'interno del documento PDF. Il valore può variare da 0 a 100 dove 0 indica la qualità più bassa ma la massima compressione e 100 indica la migliore qualità ma la compressione minima.

--------------------

Il valore predefinito è 90.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Ottiene o imposta le impostazioni della pagina per ogni pagina nel documento. Per impostazione predefinita dipende da CurrentUICulture, \*US cultures hanno impostazione letter, le altre hanno impostazione A4.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Ottiene o imposta l'algoritmo utilizzato per la divisione delle pagine.

Valore: Il `PageSplittingAlgorithm`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

