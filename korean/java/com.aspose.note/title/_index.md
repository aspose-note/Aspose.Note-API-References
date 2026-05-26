---
title: "Title"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "제목을 나타냅니다."
type: docs
weight: 95
url: /ko/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

제목을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Title()](#Title--) | `Title` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 노드 유형별로 모든 자식 노드를 가져옵니다. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | 수평 오프셋을 가져오거나 설정합니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getTitleDate()](#getTitleDate--) | 제목에 표시되는 날짜의 문자열 표현을 가져오거나 설정합니다. |
| [getTitleText()](#getTitleText--) | 제목의 텍스트를 가져오거나 설정합니다. |
| [getTitleTime()](#getTitleTime--) | 제목에 표시되는 시간의 문자열 표현을 가져오거나 설정합니다. |
| [getVerticalOffset()](#getVerticalOffset--) | 수직 오프셋을 가져오거나 설정합니다. |
| [isComposite()](#isComposite--) | 이 노드가 복합 노드인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | [Title](../../com.aspose.note/title) 의 자식 노드를 순회하는 열거자를 반환합니다. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 수평 오프셋을 가져오거나 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | 제목에 표시되는 날짜의 문자열 표현을 가져오거나 설정합니다. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | 제목의 텍스트를 가져오거나 설정합니다. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | 제목에 표시되는 시간의 문자열 표현을 가져오거나 설정합니다. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 수직 오프셋을 가져오거나 설정합니다. |
### Title() {#Title--}
```
public Title()
```


`Title` 클래스의 새 인스턴스를 초기화합니다.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


노드 유형별로 모든 자식 노드를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 자식 노드의 목록입니다.

`T1`: 반환된 목록에 있는 요소의 유형입니다.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 유형 | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


수평 오프셋을 가져오거나 설정합니다.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


제목에 표시되는 날짜의 문자열 표현을 가져오거나 설정합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


제목의 텍스트를 가져오거나 설정합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


제목에 표시되는 시간의 문자열 표현을 가져오거나 설정합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


수직 오프셋을 가져오거나 설정합니다.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


이 노드가 복합 노드인지 여부를 나타내는 값을 가져옵니다. true인 경우 노드는 자식 노드를 가질 수 있습니다.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


[Title](../../com.aspose.note/title) 의 자식 노드를 순회하는 열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
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

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


제목에 표시되는 날짜의 문자열 표현을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


제목의 텍스트를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


제목에 표시되는 시간의 문자열 표현을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


수직 오프셋을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

