---
title: "OutlineElement"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un OutlineElement."
type: docs
weight: 67
url: /it/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Rappresenta un OutlineElement.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Inizializza una nuova istanza della classe `OutlineElement`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Ottiene l'autore più recente di un elemento di outline. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Ottiene l'autore originale di un elemento di outline. |
| [getCreationTime()](#getCreationTime--) | Ottiene o imposta l'ora di creazione. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getNumberList()](#getNumberList--) | Ottiene o imposta lo stile per l'intestazione dell'elenco numerato. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Ottiene o imposta l'ora di creazione. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Ottiene o imposta lo stile per l'intestazione dell'elenco numerato. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Inizializza una nuova istanza della classe `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Ottiene l'autore più recente di un elemento di outline.

Valore: L'autore più recente.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Ottiene l'autore originale di un elemento di outline.

Valore: L'autore originale.

**Returns:**
java.lang.String
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
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Ottiene o imposta lo stile per l'intestazione dell'elenco numerato.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
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

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Ottiene o imposta lo stile per l'intestazione dell'elenco numerato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

