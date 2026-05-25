---
title: "TableCell"
second_title: "Aspose.Note for Java API Reference"
description: "Represents a table cell."
type: docs
weight: 88
url: /hi/java/com.aspose.note/tablecell/
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
| [TableCell()](#TableCell--) | `TableCell` क्लास की एक नई इंस्टेंस को प्रारंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getBackgroundColor()](#getBackgroundColor--) | पृष्ठभूमि रंग प्राप्त करता है। |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getMaxWidth()](#getMaxWidth--) | अधिकतम चौड़ाई प्राप्त करता है। |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | पृष्ठभूमि रंग सेट करता है। |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
### TableCell() {#TableCell--}
```
public TableCell()
```


`TableCell` क्लास की एक नई इंस्टेंस को प्रारंभ करता है।

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


पृष्ठभूमि रंग प्राप्त करता है।

**Returns:**
java.awt.Color
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
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


अधिकतम चौड़ाई प्राप्त करता है।

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


पृष्ठभूमि रंग सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

