---
title: "IndentatedNode"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die Basisklasse für Knoten mit relativer Einrückung für Kindknoten."
type: docs
weight: 37
url: /de/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

Die Basisklasse für Knoten mit relativer Einrückung für Kindknoten.

`T`: Der Typ der Elemente im zusammengesetzten Knoten.

T :
Self :
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Liest oder setzt die Einzugsposition. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Ermittelt die Anzahl der Elemente, die im RgOutlineIndentDistance-Array summiert werden, um die Einzugsgröße zu erhalten. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Liest oder setzt die Einzugsposition. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Liest oder setzt die Einzugsposition.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Ermittelt die Anzahl der Elemente, die im RgOutlineIndentDistance-Array summiert werden, um die Einzugsgröße zu erhalten.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Liest oder setzt die Einzugsposition.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

**Returns:**
Self
