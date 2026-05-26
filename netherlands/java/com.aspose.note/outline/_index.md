---
title: "Outline"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een overzicht voor."
type: docs
weight: 66
url: /nl/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Stelt een overzicht voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Outline()](#Outline--) | Initialiseert een nieuw exemplaar van de [Outline](../../com.aspose.note/outline) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Haalt op of afstammelingen van de outline verplaatst kunnen worden. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Haalt op of stelt de horizontale offset in. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getMaxHeight()](#getMaxHeight--) | Haalt op of stelt de maximale hoogte in. |
| [getMaxWidth()](#getMaxWidth--) | Haalt op of stelt de maximale breedte in. |
| [getMinWidth()](#getMinWidth--) | Haalt op of stelt de minimale breedte in. |
| [getReservedWidth()](#getReservedWidth--) | Haalt op of stelt de gereserveerde breedte in. |
| [getVerticalOffset()](#getVerticalOffset--) | Haalt op of stelt de verticale offset in. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Haalt op of afstammelingen van de outline verplaatst kunnen worden. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Haalt op of stelt de horizontale offset in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Haalt op of stelt de maximale hoogte in. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Haalt op of stelt de maximale breedte in. |
| [setMinWidth(float value)](#setMinWidth-float-) | Haalt op of stelt de minimale breedte in. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Haalt op of stelt de gereserveerde breedte in. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Haalt op of stelt de verticale offset in. |
### Outline() {#Outline--}
```
public Outline()
```


Initialiseert een nieuw exemplaar van de [Outline](../../com.aspose.note/outline) klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Haalt op of afstammelingen van de outline verplaatst kunnen worden.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Haalt op of stelt de horizontale offset in.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Haalt de hoeveelheid items op die opgeteld moeten worden in de RgOutlineIndentDistance-array om de inspronggrootte te verkrijgen.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Haalt op of stelt de maximale hoogte in.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Haalt op of stelt de maximale breedte in.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Haalt op of stelt de minimale breedte in.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Haalt op of stelt de gereserveerde breedte in.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Haalt op of stelt de verticale offset in.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Haalt op of afstammelingen van de outline verplaatst kunnen worden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Haalt op of stelt de horizontale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Haalt op of stelt de maximale hoogte in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Haalt op of stelt de maximale breedte in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Haalt op of stelt de minimale breedte in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Haalt op of stelt de gereserveerde breedte in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Haalt op of stelt de verticale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

