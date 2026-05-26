---
title: "PdfSaveOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Permite especificar opciones adicionales al renderizar páginas de documentos a PDF."
type: docs
weight: 77
url: /es/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Permite especificar opciones adicionales al renderizar páginas de documentos a PDF.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Inicializa una nueva instancia de la clase `PdfSaveOptions`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Obtiene el tipo de compresión aplicado a las imágenes en el archivo PDF. |
| [getJpegQuality()](#getJpegQuality--) | Obtiene un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. |
| [getPageSettings()](#getPageSettings--) | Obtiene o establece la configuración de página para cada página del documento. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Obtiene o establece el algoritmo usado para la división de páginas. |
| [setImageCompression(int value)](#setImageCompression-int-) | Establece el tipo de compresión aplicado a las imágenes en el archivo PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Establece un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Obtiene o establece la configuración de página para cada página del documento. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Obtiene o establece el algoritmo usado para la división de páginas. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Inicializa una nueva instancia de la clase `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Obtiene el tipo de compresión aplicado a las imágenes en el archivo PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Obtiene un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. El valor puede variar de 0 a 100 donde 0 significa la peor calidad pero máxima compresión y 100 significa la mejor calidad pero mínima compresión.

--------------------

El valor predeterminado es 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Obtiene o establece la configuración de página para cada página del documento. Por defecto depende de CurrentUICulture, \*US cultures tienen configuración de carta, otras tienen configuración A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Obtiene o establece el algoritmo usado para la división de páginas.

Valor: El `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Establece el tipo de compresión aplicado a las imágenes en el archivo PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Establece un valor que determina la calidad de las imágenes JPEG dentro del documento PDF. El valor puede variar de 0 a 100 donde 0 significa la peor calidad pero máxima compresión y 100 significa la mejor calidad pero mínima compresión.

--------------------

El valor predeterminado es 90.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Obtiene o establece la configuración de página para cada página del documento. Por defecto depende de CurrentUICulture, \*US cultures tienen configuración de carta, otras tienen configuración A4.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Obtiene o establece el algoritmo usado para la división de páginas.

Valor: El `PageSplittingAlgorithm`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

