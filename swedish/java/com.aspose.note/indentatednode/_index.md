---
title: "IndentatedNode"
second_title: "Aspose.Note for Java API-referens"
description: "Grundklassen för noder med relativ indentering för underordnade noder."
type: docs
weight: 37
url: /sv/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

Grundklassen för noder med relativ indentering för underordnade noder.

`T`: Typen av element i den sammansatta noden.

T :
Self :
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Hämtar eller anger indragningspositionen. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Hämtar antalet objekt som ska summeras i RgOutlineIndentDistance-arrayen för att få indragningsstorlek. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Hämtar eller anger indragningspositionen. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Hämtar eller anger indragningspositionen.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Hämtar antalet objekt som ska summeras i RgOutlineIndentDistance-arrayen för att få indragningsstorlek.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Hämtar eller anger indragningspositionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

**Returns:**
Self
