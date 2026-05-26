---
title: "Table"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "표를 나타냅니다."
type: docs
weight: 87
url: /ko/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

표를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Table()](#Table--) | `Table` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getColumns()](#getColumns--) | 테이블의 열을 가져옵니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getTags()](#getTags--) | 테이블의 모든 태그 목록을 가져옵니다. |
| [isBordersVisible()](#isBordersVisible--) | 테이블 테두리가 표시되는지 여부를 나타내는 값을 가져옵니다. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | 테이블 테두리가 표시되는지 여부를 나타내는 값을 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
### Table() {#Table--}
```
public Table()
```


`Table` 클래스의 새 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


테이블의 열을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


테이블의 모든 태그 목록을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


테이블 테두리가 표시되는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


테이블 테두리가 표시되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

