---
title: "ノード"
second_title: "Aspose.Note for Java API リファレンス"
description: "Aspose.Note ドキュメントのすべてのノードの基底クラスです。"
type: docs
weight: 51
url: /ja/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Aspose.Note ドキュメントのすべてのノードの基底クラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getDocument()](#getDocument--) | ノードのドキュメントを取得します。 |
| [getNextSibling()](#getNextSibling--) | 同じノードツリー階層の次のノードを取得します。 |
| [getNodeId()](#getNodeId--) | ノードの ID を取得します。 |
| [getNodeType()](#getNodeType--) | ノードのタイプを取得します。 |
| [getParentNode()](#getParentNode--) | 親ノードを取得します。 |
| [getPreviousSibling()](#getPreviousSibling--) | 同じノードツリー階層の前のノードを取得します。 |
| [isComposite()](#isComposite--) | このノードが複合ノードかどうかを示す値を取得します。 |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


ノードのドキュメントを取得します。

値: ドキュメント。

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


同じノードツリー階層の次のノードを取得します。

値: 次の兄弟要素。

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


ノードの ID を取得します。

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


ノードのタイプを取得します。

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


親ノードを取得します。

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


同じノードツリー階層の前のノードを取得します。

値: 前の兄弟要素。

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


このノードが複合ノードかどうかを示す値を取得します。true の場合、ノードは子ノードを持つことができます。

**Returns:**
boolean
