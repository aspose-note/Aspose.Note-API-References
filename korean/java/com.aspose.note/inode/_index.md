---
title: "INode"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "Aspose.Note 문서의 모든 노드에 대한 인터페이스입니다."
type: docs
weight: 102
url: /ko/java/com.aspose.note/inode/
---
```
public interface INode
```

Aspose.Note 문서의 모든 노드에 대한 인터페이스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) |  |
| [getNextSibling()](#getNextSibling--) |  |
| [getPreviousSibling()](#getPreviousSibling--) |  |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) |  |

### getNextSibling() {#getNextSibling--}
```
public abstract INode getNextSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
### getPreviousSibling() {#getPreviousSibling--}
```
public abstract INode getPreviousSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
