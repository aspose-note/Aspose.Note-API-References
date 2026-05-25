---
title: "Immagine"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un'immagine."
type: docs
weight: 33
url: /it/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Rappresenta un'immagine.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Inizializza una nuova istanza della classe `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Inizializza una nuova istanza della classe `Image`. |
| [Image()](#Image--) | Inizializza una nuova istanza della classe `Image`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getAlignment()](#getAlignment--) | Ottiene l'allineamento. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Ottiene un corpo e un testo alternativo per l'immagine. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Ottiene un titolo del testo alternativo per l'immagine. |
| [getBytes()](#getBytes--) | Ottiene l'archivio dei dati dell'immagine. |
| [getFileName()](#getFileName--) | Ottiene il nome del file. |
| [getFilePath()](#getFilePath--) | Ottiene il percorso del file immagine. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'immagine. |
| [getHeight()](#getHeight--) | Ottiene l'altezza. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Ottiene lo spostamento orizzontale. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Ottiene il collegamento ipertestuale associato all'immagine. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene l'ora dell'ultima modifica. |
| [getOriginalHeight()](#getOriginalHeight--) | Ottiene l'altezza originale. |
| [getOriginalWidth()](#getOriginalWidth--) | Ottiene la larghezza originale. |
| [getTags()](#getTags--) | Ottiene l'elenco di tutti i tag di un'immagine. |
| [getVerticalOffset()](#getVerticalOffset--) | Ottiene lo spostamento verticale. |
| [getWidth()](#getWidth--) | Ottiene la larghezza. |
| [isBackground()](#isBackground--) | Ottiene se l'immagine è un'immagine di sfondo. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Sostituisce i dati dell'immagine corrente con i dati dell'oggetto Image fornito. |
| [setAlignment(int value)](#setAlignment-int-) | Imposta l'allineamento. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Imposta un corpo e un testo alternativo per l'immagine. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Imposta un titolo del testo alternativo per l'immagine. |
| [setBackground(boolean value)](#setBackground-boolean-) | Ottiene se l'immagine è un'immagine di sfondo. |
| [setHeight(float value)](#setHeight-float-) | Imposta l'altezza. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Imposta lo spostamento orizzontale. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Imposta il collegamento ipertestuale associato all'immagine. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Imposta l'ora dell'ultima modifica. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Imposta lo spostamento verticale. |
| [setWidth(float value)](#setWidth-float-) | Imposta la larghezza. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Inizializza una nuova istanza della classe `Image`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | java.lang.String | Una stringa che contiene il percorso al file da cui creare l'`Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Inizializza una nuova istanza della classe `Image`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Un nome dell'immagine. |
| imageStream | java.io.InputStream | Uno stream che contiene l'immagine. |

### Image() {#Image--}
```
public Image()
```


Inizializza una nuova istanza della classe `Image`.

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


Ottiene un corpo e un testo alternativo per l'immagine.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Ottiene un titolo del testo alternativo per l'immagine.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Ottiene l'archivio dei dati dell'immagine.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Ottiene il nome del file.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Ottiene il percorso del file immagine.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Ottiene il formato dell'immagine.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Ottiene l'altezza. Questa è l'altezza reale dell'immagine nel documento MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Ottiene lo spostamento orizzontale.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Ottiene il collegamento ipertestuale associato all'immagine.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Ottiene l'altezza originale. Questa è la larghezza originale dell'immagine, prima del ridimensionamento.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Ottiene la larghezza originale. Questa è la larghezza originale dell'immagine, prima del ridimensionamento.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ottiene l'elenco di tutti i tag di un'immagine.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Ottiene lo spostamento verticale.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Ottiene la larghezza. Questa è la larghezza reale dell'immagine nel documento MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Ottiene se l'immagine è un'immagine di sfondo.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Sostituisce i dati dell'immagine corrente con i dati dell'oggetto Image fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Imposta l'allineamento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Imposta un corpo e un testo alternativo per l'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Imposta un titolo del testo alternativo per l'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Ottiene se l'immagine è un'immagine di sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Imposta l'altezza. Questa è l'altezza reale dell'immagine nel documento MS OneNote.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Imposta lo spostamento orizzontale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Imposta il collegamento ipertestuale associato all'immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Imposta lo spostamento verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Imposta la larghezza. Questa è la larghezza reale dell'immagine nel documento MS OneNote.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

