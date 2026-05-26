---
title: "IndentatedNode"
second_title: "Aspose.Note for Java API-referentie"
description: "De basis-klasse voor knooppunten met relatieve inspringing voor onderliggende knooppunten."
type: docs
weight: 37
url: /nl/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

De basis-klasse voor knooppunten met relatieve inspringing voor onderliggende knooppunten.

`T`: Het type elementen in het samengestelde knooppunt.

T :
Self :
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Haalt op of stelt de insprongpositie in. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Haalt de hoeveelheid items op die opgeteld moeten worden in de RgOutlineIndentDistance-array om de inspronggrootte te verkrijgen. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Haalt op of stelt de insprongpositie in. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Haalt op of stelt de insprongpositie in.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Haalt de hoeveelheid items op die opgeteld moeten worden in de RgOutlineIndentDistance-array om de inspronggrootte te verkrijgen.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Haalt op of stelt de insprongpositie in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

**Returns:**
Self
