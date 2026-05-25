---
title: "NodoIndentato"
second_title: "Riferimento API di Aspose.Note per Java"
description: "La classe di base per i nodi con rientro relativo per i nodi figlio."
type: docs
weight: 37
url: /it/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

La classe di base per i nodi con rientro relativo per i nodi figlio.

`T`: Il tipo di elementi nel nodo composito.

T :
Self :
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Ottiene o imposta la posizione dell'indentazione. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Ottiene il numero di elementi da sommare nell'array RgOutlineIndentDistance per ottenere la dimensione dell'indentazione. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Ottiene o imposta la posizione dell'indentazione. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Ottiene o imposta la posizione dell'indentazione.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Ottiene il numero di elementi da sommare nell'array RgOutlineIndentDistance per ottenere la dimensione dell'indentazione.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Ottiene o imposta la posizione dell'indentazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

**Returns:**
Self
