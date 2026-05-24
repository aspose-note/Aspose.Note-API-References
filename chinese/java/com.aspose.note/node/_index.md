---
title: "Node"
second_title: "Aspose.Note for Java API 参考"
description: "Aspose.Note 文档中所有节点的基类。"
type: docs
weight: 51
url: /zh/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Aspose.Note 文档中所有节点的基类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getDocument()](#getDocument--) | 获取节点的文档。 |
| [getNextSibling()](#getNextSibling--) | 获取同一节点树层级的下一个节点。 |
| [getNodeId()](#getNodeId--) | 获取节点的 ID。 |
| [getNodeType()](#getNodeType--) | 获取节点类型。 |
| [getParentNode()](#getParentNode--) | 获取父节点。 |
| [getPreviousSibling()](#getPreviousSibling--) | 获取同一节点树层级的上一个节点。 |
| [isComposite()](#isComposite--) | 获取指示此节点是否为复合节点的值。 |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


获取节点的文档。

值：文档。

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


获取同一节点树层级的下一个节点。

值：下一个兄弟节点。

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


获取节点的 ID。

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


获取节点类型。

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


获取父节点。

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


获取同一节点树层级的上一个节点。

值：上一个兄弟节点。

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


获取指示此节点是否为复合节点的值。如果为 true，则该节点可以拥有子节点。

**Returns:**
boolean
