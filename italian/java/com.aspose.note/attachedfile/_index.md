---
title: "AttachedFile"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un file allegato."
type: docs
weight: 11
url: /it/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Rappresenta un file allegato.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Inizializza una nuova istanza della classe `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Inizializza una nuova istanza della classe `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Inizializza una nuova istanza della classe `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Inizializza una nuova istanza della classe `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Inizializza una nuova istanza della classe `AttachedFile`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getAlignment()](#getAlignment--) | Ottiene l'allineamento. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Ottiene o imposta il corpo o un testo alternativo per l'icona del file allegato. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Ottiene o imposta un titolo del testo alternativo per l'icona del file allegato. |
| [getBytes()](#getBytes--) | Ottiene i dati binari per un file incorporato. |
| [getExtension()](#getExtension--) | Ottiene l'estensione di un file incorporato. |
| [getFileName()](#getFileName--) | Ottiene il nome del file incorporato. |
| [getFilePath()](#getFilePath--) | Ottiene il percorso del file originale. |
| [getHeight()](#getHeight--) | Ottiene l'altezza originale dell'icona del file incorporato. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Ottiene lo spostamento orizzontale. |
| [getIcon()](#getIcon--) | Ottiene i dati binari per l'icona associata al file incorporato. |
| [getIconExtension()](#getIconExtension--) | Ottiene l'estensione dell'icona. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene l'ora dell'ultima modifica. |
| [getMaxHeight()](#getMaxHeight--) | Ottiene l'altezza massima per visualizzare l'icona del file incorporato. |
| [getMaxWidth()](#getMaxWidth--) | Ottiene la larghezza massima per visualizzare l'icona del file incorporato. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Ottiene i dati sull'errore verificatosi durante l'accesso al file. |
| [getTags()](#getTags--) | Ottiene l'elenco dei tag di un file allegato. |
| [getText()](#getText--) | Ottiene la rappresentazione testuale del file incorporato. |
| [getVerticalOffset()](#getVerticalOffset--) | Ottiene lo spostamento verticale. |
| [getWidth()](#getWidth--) | Ottiene la larghezza originale dell'icona del file incorporato. |
| [isPrintout()](#isPrintout--) | Ottiene un valore che indica se la visualizzazione del file è una stampa. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Ottiene un valore che indica se la dimensione dell'icona è stata esplicitamente aggiornata dall'utente. |
| [setAlignment(int value)](#setAlignment-int-) | Imposta l'allineamento. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Ottiene o imposta il corpo o un testo alternativo per l'icona del file allegato. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Ottiene o imposta un titolo del testo alternativo per l'icona del file allegato. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Imposta lo spostamento orizzontale. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Imposta l'ora dell'ultima modifica. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Imposta l'altezza massima per visualizzare l'icona del file incorporato. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Imposta la larghezza massima per visualizzare l'icona del file incorporato. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Imposta un valore che indica se la visualizzazione del file è una stampa. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Imposta un valore che indica se la dimensione dell'icona è stata esplicitamente aggiornata dall'utente. |
| [setText(String value)](#setText-java.lang.String-) | Imposta la rappresentazione testuale del file incorporato. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Imposta lo spostamento verticale. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Inizializza una nuova istanza della classe `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Una stringa che contiene il percorso al file da cui creare il `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Inizializza una nuova istanza della classe `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Una stringa che contiene il percorso al file da cui creare il `AttachedFile`. |
| icona | java.io.InputStream | Un'icona per il file allegato. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Inizializza una nuova istanza della classe `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Un nome del file allegato. |
| attachedFileStream | java.io.InputStream | Uno stream che contiene i byte del file allegato. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Inizializza una nuova istanza della classe `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Un nome del file allegato. |
| attachedFileStream | java.io.InputStream | Uno stream che contiene i byte del file allegato. |
| icona | java.io.InputStream | Un'icona per il file allegato. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Un formato dell'icona del file allegato. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Inizializza una nuova istanza della classe `AttachedFile`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Ottiene l'allineamento.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Ottiene o imposta il corpo o un testo alternativo per l'icona del file allegato.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Ottiene o imposta un titolo del testo alternativo per l'icona del file allegato.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Ottiene i dati binari per un file incorporato.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Ottiene l'estensione di un file incorporato.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Ottiene il nome del file incorporato.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Ottiene il percorso del file originale.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Ottiene l'altezza originale dell'icona del file incorporato.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Ottiene lo spostamento orizzontale.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Ottiene i dati binari per l'icona associata al file incorporato.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Ottiene l'estensione dell'icona.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Ottiene l'altezza massima per visualizzare l'icona del file incorporato.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Ottiene la larghezza massima per visualizzare l'icona del file incorporato.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Ottiene i dati sull'errore verificatosi durante l'accesso al file.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ottiene l'elenco dei tag di un file allegato.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Restituisce la rappresentazione testuale del file incorporato. La stringa NON DEVE contenere alcun carattere con valore 10 (line feed) o 13 (carriage return).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Ottiene lo spostamento verticale.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Ottiene la larghezza originale dell'icona del file incorporato.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Ottiene un valore che indica se la visualizzazione del file è una stampa.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Ottiene un valore che indica se la dimensione dell'icona è stata esplicitamente aggiornata dall'utente.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Imposta l'allineamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Valore di Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Ottiene o imposta il corpo o un testo alternativo per l'icona del file allegato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Ottiene o imposta un titolo del testo alternativo per l'icona del file allegato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Imposta lo spostamento orizzontale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | Valore di Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | Valore di Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Imposta l'altezza massima per visualizzare l'icona del file incorporato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | Valore dell'altezza massima. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Imposta la larghezza massima per visualizzare l'icona del file incorporato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | Valore della larghezza massima. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Imposta un valore che indica se la visualizzazione del file è una stampa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | Nuovo valore. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Imposta un valore che indica se la dimensione dell'icona è stata esplicitamente aggiornata dall'utente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | Nuovo valore. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta la rappresentazione testuale del file incorporato. La stringa NON DEVE contenere alcun carattere con valore 10 (line feed) o 13 (carriage return).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | Valore di Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Imposta lo spostamento verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float | Valore di Offset. |

