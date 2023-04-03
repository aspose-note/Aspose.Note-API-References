---
title: Outline
second_title: Aspose.Note for Java API Reference
description: Represents a Outline.
type: docs
weight: 56
url: /java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Represents a Outline.
## Constructors

| Constructor | Description |
| --- | --- |
| [Outline()](#Outline--) | Initializes a new instance of the [Outline](../../com.aspose.note/outline) class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [getMaxWidth()](#getMaxWidth--) | Gets or sets the max width. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Gets or sets the max width. |
| [getMinWidth()](#getMinWidth--) | Gets or sets the min width. |
| [setMinWidth(float value)](#setMinWidth-float-) | Gets or sets the min width. |
| [getMaxHeight()](#getMaxHeight--) | Gets or sets the max height. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Gets or sets the max height. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets or sets the horizontal offset. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Gets or sets the horizontal offset. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets or sets the vertical offset. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Gets or sets the vertical offset. |
| [getReservedWidth()](#getReservedWidth--) | Gets or sets the reserved width. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Gets or sets the reserved width. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Gets whether descendants of the outline can be moved. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Gets whether descendants of the outline can be moved. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### Outline() {#Outline--}
```
public Outline()
```


Initializes a new instance of the [Outline](../../com.aspose.note/outline) class.

### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Gets or sets the max width.

**Returns:**
float
### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Gets or sets the max width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Gets or sets the min width.

**Returns:**
float
### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Gets or sets the min width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Gets or sets the max height.

**Returns:**
float
### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Gets or sets the max height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Gets or sets the horizontal offset.

**Returns:**
float
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Gets or sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Gets or sets the vertical offset.

**Returns:**
float
### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Gets or sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Gets or sets the reserved width.

**Returns:**
float
### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Gets or sets the reserved width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Gets whether descendants of the outline can be moved.

**Returns:**
boolean
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Gets whether descendants of the outline can be moved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size.

**Returns:**
int
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

