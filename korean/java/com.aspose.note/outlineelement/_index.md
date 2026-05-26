---
title: "OutlineElement"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "OutlineElement를 나타냅니다."
type: docs
weight: 67
url: /ko/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

OutlineElement를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | `OutlineElement` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | 아웃라인 요소의 가장 최근 작성자를 가져옵니다. |
| [getAuthorOriginal()](#getAuthorOriginal--) | 아웃라인 요소의 원본 작성자를 가져옵니다. |
| [getCreationTime()](#getCreationTime--) | 생성 시간을 가져오거나 설정합니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getNumberList()](#getNumberList--) | 번호 매기기 목록 헤더의 스타일을 가져오거나 설정합니다. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 생성 시간을 가져오거나 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | 번호 매기기 목록 헤더의 스타일을 가져오거나 설정합니다. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


`OutlineElement` 클래스의 새 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


아웃라인 요소의 가장 최근 작성자를 가져옵니다.

값: 가장 최근 작성자.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


아웃라인 요소의 원본 작성자를 가져옵니다.

값: 원본 작성자.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


생성 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


번호 매기기 목록 헤더의 스타일을 가져오거나 설정합니다.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


생성 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


번호 매기기 목록 헤더의 스타일을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

