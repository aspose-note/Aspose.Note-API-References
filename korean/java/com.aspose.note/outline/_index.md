---
title: "개요"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "개요를 나타냅니다."
type: docs
weight: 66
url: /ko/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

개요를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Outline()](#Outline--) | 새 인스턴스를 초기화합니다 [Outline](../../com.aspose.note/outline) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | 개요의 하위 항목을 이동할 수 있는지 여부를 가져옵니다. |
| [getHorizontalOffset()](#getHorizontalOffset--) | 수평 오프셋을 가져오거나 설정합니다. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getMaxHeight()](#getMaxHeight--) | 최대 높이를 가져오거나 설정합니다. |
| [getMaxWidth()](#getMaxWidth--) | 최대 너비를 가져오거나 설정합니다. |
| [getMinWidth()](#getMinWidth--) | 최소 너비를 가져오거나 설정합니다. |
| [getReservedWidth()](#getReservedWidth--) | 예약된 너비를 가져오거나 설정합니다. |
| [getVerticalOffset()](#getVerticalOffset--) | 수직 오프셋을 가져오거나 설정합니다. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | 개요의 하위 항목을 이동할 수 있는지 여부를 가져옵니다. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 수평 오프셋을 가져오거나 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 최대 높이를 가져오거나 설정합니다. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 최대 너비를 가져오거나 설정합니다. |
| [setMinWidth(float value)](#setMinWidth-float-) | 최소 너비를 가져오거나 설정합니다. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | 예약된 너비를 가져오거나 설정합니다. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 수직 오프셋을 가져오거나 설정합니다. |
### Outline() {#Outline--}
```
public Outline()
```


새 인스턴스를 초기화합니다 [Outline](../../com.aspose.note/outline) 클래스.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


개요의 하위 항목을 이동할 수 있는지 여부를 가져옵니다.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


수평 오프셋을 가져오거나 설정합니다.

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


최대 높이를 가져오거나 설정합니다.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


최대 너비를 가져오거나 설정합니다.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


최소 너비를 가져오거나 설정합니다.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


예약된 너비를 가져오거나 설정합니다.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


수직 오프셋을 가져오거나 설정합니다.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


개요의 하위 항목을 이동할 수 있는지 여부를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


수평 오프셋을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


최대 높이를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


최대 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


최소 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


예약된 너비를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


수직 오프셋을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

