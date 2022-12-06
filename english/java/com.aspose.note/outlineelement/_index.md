---
title: OutlineElement
second_title: Aspose.Note for Java API Reference
description: Represents a OutlineElement.
type: docs
weight: 53
url: /java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Represents a OutlineElement.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineElement(Document document)](#OutlineElement-com.aspose.note.Document-) | Initializes a new instance of the  OutlineElement  class. |
| [OutlineElement()](#OutlineElement--) | Initializes a new instance of the  OutlineElement  class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [getNumberList()](#getNumberList--) | Gets or sets the style for the numbered list header. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Gets or sets the style for the numbered list header. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### OutlineElement(Document document) {#OutlineElement-com.aspose.note.Document-}
```
public OutlineElement(Document document)
```


Initializes a new instance of the  OutlineElement  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The parent document of the outline element. |

### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initializes a new instance of the  OutlineElement  class.

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

### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Gets or sets the creation time.

**Returns:**
java.util.Date
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Gets or sets the creation time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Gets or sets the style for the numbered list header.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Gets or sets the style for the numbered list header.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

