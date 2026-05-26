---
title: "노드"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "Aspose.Note 문서의 모든 노드에 대한 기본 클래스입니다."
type: docs
weight: 51
url: /ko/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Aspose.Note 문서의 모든 노드에 대한 기본 클래스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getDocument()](#getDocument--) | 노드의 문서를 가져옵니다. |
| [getNextSibling()](#getNextSibling--) | 같은 노드 트리 레벨에 있는 다음 노드를 가져옵니다. |
| [getNodeId()](#getNodeId--) | 노드의 ID를 가져옵니다. |
| [getNodeType()](#getNodeType--) | 노드 유형을 가져옵니다. |
| [getParentNode()](#getParentNode--) | 부모 노드를 가져옵니다. |
| [getPreviousSibling()](#getPreviousSibling--) | 같은 노드 트리 레벨에 있는 이전 노드를 가져옵니다. |
| [isComposite()](#isComposite--) | 이 노드가 복합 노드인지 여부를 나타내는 값을 가져옵니다. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


노드의 문서를 가져옵니다.

값: 문서.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


같은 노드 트리 레벨에 있는 다음 노드를 가져옵니다.

값: 다음 형제.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


노드의 ID를 가져옵니다.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


노드 유형을 가져옵니다.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


부모 노드를 가져옵니다.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


같은 노드 트리 레벨에 있는 이전 노드를 가져옵니다.

값: 이전 형제.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


이 노드가 복합 노드인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드는 자식 노드를 가질 수 있습니다.

**Returns:**
boolean
