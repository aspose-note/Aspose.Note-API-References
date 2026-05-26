---
title: "InkDrawing"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "그려진 콘텐츠를 포함하는 잉크 노드를 나타냅니다."
type: docs
weight: 38
url: /ko/java/com.aspose.note/inkdrawing/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.InkNode](../../com.aspose.note/inknode)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class InkDrawing extends InkNode implements IPageChildNode
```

그려진 콘텐츠를 포함하는 잉크 노드를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getHorizontalOffset()](#getHorizontalOffset--) | 수평 오프셋을 가져옵니다. |
| [getVerticalOffset()](#getVerticalOffset--) | 수직 오프셋을 가져옵니다. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 수평 오프셋을 설정합니다. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 수직 오프셋을 설정합니다. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 다음으로부터 파생된 클래스인 [DocumentVisitor](../../com.aspose.note/documentvisitor)의 객체. |

### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


수평 오프셋을 가져옵니다.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


수직 오프셋을 가져옵니다.

**Returns:**
float
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


수평 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


수직 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

