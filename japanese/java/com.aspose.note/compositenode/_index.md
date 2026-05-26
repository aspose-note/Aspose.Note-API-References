---
title: "CompositeNode"
second_title: "Aspose.Note for Java API リファレンス"
description: "他のノードを含むことができるノードの基本ジェネリッククラスです。"
type: docs
weight: 15
url: /ja/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

他のノードを含むことができるノードの基本ジェネリッククラスです。

`T`: 複合ノード内の要素の型です。

T :
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | このノードの子ノードリストの先頭にノードを追加します。 |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | このノードの子ノードリストの末尾にノードを追加します。 |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | ノードのタイプで子ノードをすべて取得します。 |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | このノードの子ノードリストの指定位置にノードを挿入します。 |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | 子ノードを削除します。 |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getFirstChild()](#getFirstChild--) | このノードの最初の子ノードを取得します。 |
| [getLastChild()](#getLastChild--) | このノードの最後の子ノードを取得します。 |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | このノードの子ノードリストの指定位置からノードのシーケンスを挿入します。 |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | このノードの子ノードリストの指定位置からノードのシーケンスを挿入します。 |
| [isComposite()](#isComposite--) | ノードが複合かどうかを確認します。 |
| [iterator()](#iterator--) | `CompositeNode\{T\}` の子ノードを列挙する列挙子を返します。 |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


このノードの子ノードリストの先頭にノードを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newChild | T1 | 追加するノードです。 |

**Returns:**
T1 - 追加されたノード。
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


このノードの子ノードリストの末尾にノードを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newChild | T1 | 追加するノードです。 |

**Returns:**
T1 - 追加されたノード。
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


ノードのタイプで子ノードをすべて取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 子ノードのリスト。

`T1`: 返されたリスト内の要素の型です。
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


このノードの子ノードリストの指定位置にノードを挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| i | int | 挿入位置 |
| newChild | T1 | 挿入するノードです。 |

**Returns:**
T1 - 追加されたノード。
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


子ノードを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldChild | T1 | 削除するノードです。 |

**Returns:**
T1 - 削除されたノード。
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


このノードの最初の子ノードを取得します。

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


このノードの最後の子ノードを取得します。

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


このノードの子ノードリストの指定位置からノードのシーケンスを挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| i | int | 挿入位置 |
| newChildren | T[] | 挿入されるノードのシーケンスです。 |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


このノードの子ノードリストの指定位置からノードのシーケンスを挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| i | int | 挿入位置 |
| newChildren | java.lang.Iterable&lt;T&gt; | 挿入されるノードのシーケンスです。 |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


ノードが複合かどうかをチェックします。true の場合、ノードは子ノードを持つことができます。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


`CompositeNode\{T\}` の子ノードを列挙する列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - `CompositeNode\{T\}` 用の `T:IEnumerator`1`。
