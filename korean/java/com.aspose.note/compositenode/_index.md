---
title: "CompositeNode"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "다른 노드를 포함할 수 있는 노드의 기본 제네릭 클래스입니다."
type: docs
weight: 15
url: /ko/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

다른 노드를 포함할 수 있는 노드의 기본 제네릭 클래스입니다.

`T`: 복합 노드의 요소 유형.

T :
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | 이 노드의 자식 노드 목록 앞에 노드를 추가합니다. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | 이 노드의 자식 노드 목록 끝에 노드를 추가합니다. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 노드 유형별로 모든 자식 노드를 가져옵니다. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | 이 노드의 자식 노드 목록에서 지정된 위치에 노드를 삽입합니다. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | 자식 노드를 제거합니다. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getFirstChild()](#getFirstChild--) | 이 노드의 첫 번째 자식 노드를 가져옵니다. |
| [getLastChild()](#getLastChild--) | 이 노드의 마지막 자식 노드를 가져옵니다. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | 이 노드의 자식 노드 목록에서 지정된 위치부터 노드 시퀀스를 삽입합니다. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | 이 노드의 자식 노드 목록에서 지정된 위치부터 노드 시퀀스를 삽입합니다. |
| [isComposite()](#isComposite--) | 노드가 복합인지 확인합니다. |
| [iterator()](#iterator--) | `CompositeNode\\{T\\}` 의 자식 노드를 반복하는 열거자를 반환합니다. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


이 노드의 자식 노드 목록 앞에 노드를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| newChild | T1 | 추가할 노드입니다. |

**Returns:**
T1 - 추가된 노드.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


이 노드의 자식 노드 목록 끝에 노드를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| newChild | T1 | 추가할 노드입니다. |

**Returns:**
T1 - 추가된 노드.
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
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


이 노드의 자식 노드 목록에서 지정된 위치에 노드를 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| i | int | 삽입 위치 |
| newChild | T1 | 삽입할 노드입니다. |

**Returns:**
T1 - 추가된 노드.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


자식 노드를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| oldChild | T1 | 제거할 노드입니다. |

**Returns:**
T1 - 제거된 노드.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


이 노드의 첫 번째 자식 노드를 가져옵니다.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


이 노드의 마지막 자식 노드를 가져옵니다.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


이 노드의 자식 노드 목록에서 지정된 위치부터 노드 시퀀스를 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| i | int | 삽입 위치 |
| newChildren | T[] | 삽입될 노드 시퀀스입니다. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


이 노드의 자식 노드 목록에서 지정된 위치부터 노드 시퀀스를 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| i | int | 삽입 위치 |
| newChildren | java.lang.Iterable&lt;T&gt; | 삽입될 노드 시퀀스입니다. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


노드가 복합인지 확인합니다. true인 경우 노드가 자식 노드를 가질 수 있습니다.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


`CompositeNode\\{T\\}` 의 자식 노드를 반복하는 열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - `CompositeNode\{T\}`에 대한 `T:IEnumerator`1`.
