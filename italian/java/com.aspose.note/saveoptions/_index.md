---
title: "SaveOptions"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Una classe base astratta che rappresenta le opzioni di salvataggio del documento per un formato particolare."
type: docs
weight: 85
url: /it/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Una classe base astratta che rappresenta le opzioni di salvataggio del documento per un formato particolare.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Ottiene o imposta le impostazioni del font da utilizzare durante il salvataggio. |
| [getPageCount()](#getPageCount--) | Ottiene o imposta il numero di pagine da salvare. |
| [getPageIndex()](#getPageIndex--) | Ottiene o imposta l'indice della prima pagina da salvare. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene o imposta il formato in cui il documento viene salvato. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Ottiene o imposta le impostazioni del font da utilizzare durante il salvataggio. |
| [setPageCount(int value)](#setPageCount-int-) | Ottiene o imposta il numero di pagine da salvare. |
| [setPageIndex(int value)](#setPageIndex-int-) | Ottiene o imposta l'indice della prima pagina da salvare. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Ottiene o imposta le impostazioni del font da utilizzare durante il salvataggio.

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Ottiene o imposta il numero di pagine da salvare. Per impostazione predefinita è \{@link int\#Int32Extensions.MaxValue\} che significa che tutte le pagine del documento verranno renderizzate.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Ottiene o imposta l'indice della prima pagina da salvare. Per impostazione predefinita è 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene o imposta il formato in cui il documento viene salvato.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Ottiene o imposta le impostazioni del font da utilizzare durante il salvataggio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Ottiene o imposta il numero di pagine da salvare. Per impostazione predefinita è \{@link int\#Int32Extensions.MaxValue\} che significa che tutte le pagine del documento verranno renderizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Ottiene o imposta l'indice della prima pagina da salvare. Per impostazione predefinita è 0.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

