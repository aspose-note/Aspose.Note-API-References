---
title: "IndentatedNode"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "자식 노드에 대한 상대 들여쓰기를 가진 노드의 기본 클래스입니다."
type: docs
weight: 37
url: /ko/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

자식 노드에 대한 상대 들여쓰기를 가진 노드의 기본 클래스입니다.

`T`: 복합 노드의 요소 유형.

T :
Self :
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | 들여쓰기 위치를 가져오거나 설정합니다. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | 들여쓰기 크기를 얻기 위해 RgOutlineIndentDistance 배열에서 합산할 항목 수를 가져옵니다. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | 들여쓰기 위치를 가져오거나 설정합니다. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


들여쓰기 위치를 가져오거나 설정합니다.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


들여쓰기 크기를 얻기 위해 RgOutlineIndentDistance 배열에서 합산할 항목 수를 가져옵니다.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


들여쓰기 위치를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

**Returns:**
Self
