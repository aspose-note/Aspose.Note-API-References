---
title: "TableCell"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta una cella di tabella."
type: docs
weight: 88
url: /it/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Rappresenta una cella di tabella.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TableCell()](#TableCell--) | Inizializza una nuova istanza della classe `TableCell`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getBackgroundColor()](#getBackgroundColor--) | Ottiene il colore di sfondo. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getMaxWidth()](#getMaxWidth--) | Ottiene la larghezza massima. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Imposta il colore di sfondo. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Inizializza una nuova istanza della classe `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Ottiene il colore di sfondo.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Ottiene il numero di elementi da sommare nell'array RgOutlineIndentDistance per ottenere la dimensione dell'indentazione.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene o imposta l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Ottiene la larghezza massima.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Imposta il colore di sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ottiene o imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

