---
title: "SaveOptions"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Una clase base abstracta que representa las opciones de guardado de documentos para un formato particular."
type: docs
weight: 85
url: /es/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Una clase base abstracta que representa las opciones de guardado de documentos para un formato particular.
## Métodos

| Método | Descripción |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Obtiene o establece la configuración de la fuente que se usará al guardar |
| [getPageCount()](#getPageCount--) | Obtiene o establece el número de páginas a guardar. |
| [getPageIndex()](#getPageIndex--) | Obtiene o establece el índice de la primera página a guardar. |
| [getSaveFormat()](#getSaveFormat--) | Obtiene o establece el formato en el que se guarda el documento. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Obtiene o establece la configuración de la fuente que se usará al guardar |
| [setPageCount(int value)](#setPageCount-int-) | Obtiene o establece el número de páginas a guardar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Obtiene o establece el índice de la primera página a guardar. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Obtiene o establece la configuración de la fuente que se usará al guardar

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtiene o establece el número de páginas a guardar. Por defecto es \{@link int\#Int32Extensions.MaxValue\} lo que significa que se renderizarán todas las páginas del documento.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Obtiene o establece el índice de la primera página a guardar. Por defecto es 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtiene o establece el formato en el que se guarda el documento.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Obtiene o establece la configuración de la fuente que se usará al guardar

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Obtiene o establece el número de páginas a guardar. Por defecto es \{@link int\#Int32Extensions.MaxValue\} lo que significa que se renderizarán todas las páginas del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Obtiene o establece el índice de la primera página a guardar. Por defecto es 0.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

