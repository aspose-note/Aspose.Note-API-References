---
title: OutlineGroup
second_title: Aspose.Note for Java API Reference
description: Represents a OutlineGroup.
type: docs
weight: 53
url: /java/com.aspose.note/outlinegroup/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineGroup extends CompositeNode<IOutlineChildNode> implements IOutlineChildNode, IOutlineElementChildNode
```

Represents a OutlineGroup.
## Constructors

| Constructor | Description |
| --- | --- |
| [OutlineGroup(Document document)](#OutlineGroup-com.aspose.note.Document-) | Initializes a new instance of the  OutlineGroup  class. |
| [OutlineGroup()](#OutlineGroup--) | Initializes a new instance of the  OutlineGroup  class. |
## Methods

| Method | Description |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Gets or sets the indent position. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Gets or sets the indent position. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### OutlineGroup(Document document) {#OutlineGroup-com.aspose.note.Document-}
```
public OutlineGroup(Document document)
```


Initializes a new instance of the  OutlineGroup  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The document of the outline group. |

### OutlineGroup() {#OutlineGroup--}
```
public OutlineGroup()
```


Initializes a new instance of the  OutlineGroup  class.

### getIndentPosition() {#getIndentPosition--}
```
public byte getIndentPosition()
```


Gets or sets the indent position.

**Returns:**
byte
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public void setIndentPosition(byte value)
```


Gets or sets the indent position.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte |  |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |
