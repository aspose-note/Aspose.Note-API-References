---
title: "Node"
second_title: "Aspose.Note for Java API Reference"
description: "The base class for all nodes of an Aspose.Note document."
type: docs
weight: 51
url: /hi/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

The base class for all nodes of an Aspose.Note document.
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getDocument()](#getDocument--) | Gets the document of the node. |
| [getNextSibling()](#getNextSibling--) | Gets the next node at the same node tree level. |
| [getNodeId()](#getNodeId--) | Gets the node's ID. |
| [getNodeType()](#getNodeType--) | नोड प्रकार प्राप्त करता है। |
| [getParentNode()](#getParentNode--) | पैरेंट नोड प्राप्त करता है। |
| [getPreviousSibling()](#getPreviousSibling--) | समान नोड ट्री स्तर पर पिछला नोड प्राप्त करता है। |
| [isComposite()](#isComposite--) | Gets a value indicating whether this node is composite. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Gets the document of the node.

मान: दस्तावेज़।

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Gets the next node at the same node tree level.

मान: अगला सहभाई।

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Gets the node's ID.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


नोड प्रकार प्राप्त करता है।

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


पैरेंट नोड प्राप्त करता है।

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


समान नोड ट्री स्तर पर पिछला नोड प्राप्त करता है।

मान: पिछला सहभाई।

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Gets a value indicating whether this node is composite. If true the node can have child nodes.

**Returns:**
boolean
