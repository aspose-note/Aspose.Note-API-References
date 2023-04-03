---
title: TableCell
second_title: Aspose.Note for Java API Reference
description: Represents a table cell.
type: docs
weight: 77
url: /java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Represents a table cell.
## Constructors

| Constructor | Description |
| --- | --- |
| [TableCell()](#TableCell--) | Initializes a new instance of the  TableCell  class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [getMaxWidth()](#getMaxWidth--) | Gets the max width. |
| [getBackgroundColor()](#getBackgroundColor--) | Gets the background color. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Sets the background color. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
### TableCell() {#TableCell--}
```
public TableCell()
```


Initializes a new instance of the  TableCell  class.

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


Gets the max width.

**Returns:**
float
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Gets the background color.

**Returns:**
java.awt.Color
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Sets the background color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Gets the amount of items to sum up in RgOutlineIndentDistance array to get indent size.

**Returns:**
int
