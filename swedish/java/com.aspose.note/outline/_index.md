---
title: "Disposition"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en översikt."
type: docs
weight: 66
url: /sv/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Representerar en översikt.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Outline()](#Outline--) | Initierar en ny instans av klassen [Outline](../../com.aspose.note/outline). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Hämtar om efterkommande till outline kan flyttas. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Hämtar eller anger den horisontella förskjutningen. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getMaxHeight()](#getMaxHeight--) | Hämtar eller anger maximal höjd. |
| [getMaxWidth()](#getMaxWidth--) | Hämtar eller anger maximal bredd. |
| [getMinWidth()](#getMinWidth--) | Hämtar eller anger minimal bredd. |
| [getReservedWidth()](#getReservedWidth--) | Hämtar eller anger reserverad bredd. |
| [getVerticalOffset()](#getVerticalOffset--) | Hämtar eller anger den vertikala förskjutningen. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Hämtar om efterkommande till outline kan flyttas. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Hämtar eller anger den horisontella förskjutningen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Hämtar eller anger maximal höjd. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Hämtar eller anger maximal bredd. |
| [setMinWidth(float value)](#setMinWidth-float-) | Hämtar eller anger minimal bredd. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Hämtar eller anger reserverad bredd. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Hämtar eller anger den vertikala förskjutningen. |
### Outline() {#Outline--}
```
public Outline()
```


Initierar en ny instans av klassen [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Hämtar om efterkommande till outline kan flyttas.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Hämtar eller anger den horisontella förskjutningen.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Hämtar antalet objekt som ska summeras i RgOutlineIndentDistance-arrayen för att få indragningsstorlek.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Hämtar eller anger maximal höjd.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Hämtar eller anger maximal bredd.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Hämtar eller anger minimal bredd.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Hämtar eller anger reserverad bredd.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Hämtar eller anger den vertikala förskjutningen.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Hämtar om efterkommande till outline kan flyttas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Hämtar eller anger den horisontella förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Hämtar eller anger maximal höjd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Hämtar eller anger maximal bredd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Hämtar eller anger minimal bredd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Hämtar eller anger reserverad bredd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Hämtar eller anger den vertikala förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

