---
title: "Page"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta una pagina."
type: docs
weight: 69
url: /it/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Rappresenta una pagina.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Page()](#Page--) | Inizializza una nuova istanza della classe `Page`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [deepClone()](#deepClone--) | Clona la pagina. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Clona la pagina. |
| [getAuthor()](#getAuthor--) | Ottiene o imposta l'autore. |
| [getBackgroundColor()](#getBackgroundColor--) | Ottiene o imposta il colore di sfondo della pagina. |
| [getCreationTime()](#getCreationTime--) | Ottiene o imposta l'ora di creazione. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getLevel()](#getLevel--) | Ottiene o imposta il livello. |
| [getMargin()](#getMargin--) | Ottiene o imposta il margine. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Ottiene o imposta il riepilogo della revisione per la pagina e i suoi nodi figli. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Ottiene la dimensione del layout della pagina visualizzata nell'editor. |
| [getSizeType()](#getSizeType--) | Ottiene o imposta il tipo di dimensione di una pagina. |
| [getTitle()](#getTitle--) | Ottiene o imposta il titolo. |
| [isConflictPage()](#isConflictPage--) | Ottiene o imposta un valore che indica se questa pagina è una pagina di conflitto. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ottiene o imposta l'autore. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Ottiene o imposta il colore di sfondo della pagina. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Ottiene o imposta un valore che indica se questa pagina è una pagina di conflitto. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Ottiene o imposta l'ora di creazione. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
| [setLevel(byte value)](#setLevel-byte-) | Ottiene o imposta il livello. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Ottiene o imposta il margine. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Ottiene o imposta il riepilogo della revisione per la pagina e i suoi nodi figli. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Imposta la dimensione del layout della pagina visualizzata nell'editor. |
| [setSizeType(int value)](#setSizeType-int-) | Ottiene o imposta il tipo di dimensione di una pagina. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Ottiene o imposta il titolo. |
### Page() {#Page--}
```
public Page()
```


Inizializza una nuova istanza della classe `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Clona la pagina.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Clona la pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cloneHistory | boolean | Specifica se la cronologia della pagina deve essere clonata.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Ottiene o imposta l'autore.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Ottiene o imposta il colore di sfondo della pagina.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Ottiene o imposta l'ora di creazione.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene o imposta l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Ottiene o imposta il livello.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Ottiene o imposta il margine.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Ottiene o imposta il riepilogo della revisione per la pagina e i suoi nodi figli.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Ottiene la dimensione del layout della pagina visualizzata nell'editor.

--------------------

Questo valore è utilizzato dall'applicazione Microsoft OneNote per visualizzare il layout sottostante della pagina quando il documento viene aperto. Non influisce comunque sulla stampa e sul salvataggio del documento. Quando la proprietà Page.SizeType è impostata su PageSizeType.SizeByContent, questa proprietà restituisce la dimensione reale del contenuto.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Ottiene o imposta il tipo di dimensione di una pagina.

--------------------

Per impostazione predefinita, una pagina si ridimensiona automaticamente. Il valore predefinito è [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Ottiene o imposta il titolo.

Valore: il `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Ottiene o imposta un valore che indica se questa pagina è una pagina di conflitto.

--------------------

La pagina di conflitto si verifica quando due utenti tentano di aggiornare lo stesso contenuto. In questo caso le modifiche del primo utente vengono scritte normalmente. Ma le modifiche dell'altro utente non possono essere unite. Pertanto viene creata una copia della pagina e contrassegnata come conflitto.

In questa versione i conflitti vengono risolti a favore delle modifiche del primo utente. Quindi, se il documento contiene pagine di conflitto, queste verranno mostrate nella cronologia ma verranno ignorate durante il salvataggio. È possibile reimpostare questa flag per salvare queste pagine nella cronologia come pagine normali.

È possibile trovare un esempio dettagliato di manipolazione della pagina di conflitto nella documentazione online.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Ottiene o imposta l'autore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Ottiene o imposta il colore di sfondo della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Ottiene o imposta un valore che indica se questa pagina è una pagina di conflitto.

--------------------

La pagina di conflitto si verifica quando due utenti tentano di aggiornare lo stesso contenuto. In questo caso le modifiche del primo utente vengono scritte normalmente. Ma le modifiche dell'altro utente non possono essere unite. Pertanto viene creata una copia della pagina e contrassegnata come conflitto.

In questa versione i conflitti vengono risolti a favore delle modifiche del primo utente. Quindi, se il documento contiene pagine di conflitto, queste verranno mostrate nella cronologia ma verranno ignorate durante il salvataggio. È possibile reimpostare questa flag per salvare queste pagine nella cronologia come pagine normali.

È possibile trovare un esempio dettagliato di manipolazione della pagina di conflitto nella documentazione online.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Ottiene o imposta l'ora di creazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ottiene o imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Ottiene o imposta il livello.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Ottiene o imposta il margine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Ottiene o imposta il riepilogo della revisione per la pagina e i suoi nodi figli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Imposta la dimensione del layout della pagina visualizzata nell'editor.

--------------------

Questo valore è utilizzato dall'applicazione Microsoft OneNote per visualizzare il layout sottostante della pagina quando il documento viene aperto. Non influisce comunque sulla stampa e sul salvataggio del documento. Quando la proprietà Page.SizeType è impostata su PageSizeType.SizeByContent, questa proprietà restituisce la dimensione reale del contenuto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Ottiene o imposta il tipo di dimensione di una pagina.

--------------------

Per impostazione predefinita, una pagina si ridimensiona automaticamente. Il valore predefinito è [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Ottiene o imposta il titolo.

Valore: il `Title`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

