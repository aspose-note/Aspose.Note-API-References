---
title: "TableCell"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "표 셀을 나타냅니다."
type: docs
weight: 88
url: /ko/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

표 셀을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TableCell()](#TableCell--) | `TableCell` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getBackgroundColor()](#getBackgroundColor--) | 배경 색상을 가져옵니다. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getMaxWidth()](#getMaxWidth--) | 최대 너비를 가져옵니다. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 배경 색상을 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
### TableCell() {#TableCell--}
```
public TableCell()
```


`TableCell` 클래스의 새 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


배경 색상을 가져옵니다.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


들여쓰기 크기를 얻기 위해 RgOutlineIndentDistance 배열에서 합산할 항목 수를 가져옵니다.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


최대 너비를 가져옵니다.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


배경 색상을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

