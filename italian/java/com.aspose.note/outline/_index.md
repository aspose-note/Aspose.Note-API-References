---
title: "Struttura"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta una struttura."
type: docs
weight: 66
url: /it/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Rappresenta una struttura.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Outline()](#Outline--) | Inizializza una nuova istanza della classe [Outline](../../com.aspose.note/outline). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Ottiene se i discendenti della struttura possono essere spostati. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Ottiene o imposta lo spostamento orizzontale. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getMaxHeight()](#getMaxHeight--) | Ottiene o imposta l'altezza massima. |
| [getMaxWidth()](#getMaxWidth--) | Ottiene o imposta la larghezza massima. |
| [getMinWidth()](#getMinWidth--) | Ottiene o imposta la larghezza minima. |
| [getReservedWidth()](#getReservedWidth--) | Ottiene o imposta la larghezza riservata. |
| [getVerticalOffset()](#getVerticalOffset--) | Ottiene o imposta lo spostamento verticale. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Ottiene se i discendenti della struttura possono essere spostati. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ottiene o imposta lo spostamento orizzontale. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Ottiene o imposta l'altezza massima. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Ottiene o imposta la larghezza massima. |
| [setMinWidth(float value)](#setMinWidth-float-) | Ottiene o imposta la larghezza minima. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Ottiene o imposta la larghezza riservata. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ottiene o imposta lo spostamento verticale. |
### Outline() {#Outline--}
```
public Outline()
```


Inizializza una nuova istanza della classe [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Ottiene se i discendenti della struttura possono essere spostati.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Ottiene o imposta lo spostamento orizzontale.

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Ottiene o imposta l'altezza massima.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Ottiene o imposta la larghezza massima.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Ottiene o imposta la larghezza minima.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Ottiene o imposta la larghezza riservata.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Ottiene o imposta lo spostamento verticale.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Ottiene se i discendenti della struttura possono essere spostati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Ottiene o imposta lo spostamento orizzontale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ottiene o imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Ottiene o imposta l'altezza massima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Ottiene o imposta la larghezza massima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Ottiene o imposta la larghezza minima.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Ottiene o imposta la larghezza riservata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Ottiene o imposta lo spostamento verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

