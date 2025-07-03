---
title: Outline
second_title: Aspose.Note for Java API Reference
description: Represents a Outline.
type: docs
weight: 66
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
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Gets whether descendants of the outline can be moved. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Gets or sets the horizontal offset. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getMaxHeight()](#getMaxHeight--) | Gets or sets the max height. |
| [getMaxWidth()](#getMaxWidth--) | Gets or sets the max width. |
| [getMinWidth()](#getMinWidth--) | Gets or sets the min width. |
| [getReservedWidth()](#getReservedWidth--) | Gets or sets the reserved width. |
| [getVerticalOffset()](#getVerticalOffset--) | Gets or sets the vertical offset. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Gets whether descendants of the outline can be moved. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Gets or sets the horizontal offset. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Gets or sets the max height. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Gets or sets the max width. |
| [setMinWidth(float value)](#setMinWidth-float-) | Gets or sets the min width. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Gets or sets the reserved width. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Gets or sets the vertical offset. |
### Outline() {#Outline--}
```
public Outline()
```


Initializes a new instance of the [Outline](../../com.aspose.note/outline) class.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Gets whether descendants of the outline can be moved.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Gets or sets the horizontal offset.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Gets or sets the max height.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Gets or sets the max width.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Gets or sets the min width.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Gets or sets the reserved width.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Gets or sets the vertical offset.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Gets whether descendants of the outline can be moved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Gets or sets the horizontal offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Gets or sets the max height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Gets or sets the max width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Gets or sets the min width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Gets or sets the reserved width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Gets or sets the vertical offset.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |

