---
title: "CompositeNode"
second_title: "Aspose.Note for Java API 参考"
description: "用于可以包含其他节点的节点的基础通用类。"
type: docs
weight: 15
url: /zh/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

用于可以包含其他节点的节点的基础通用类。

`T`：复合节点中元素的类型。

T :
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | 将节点添加到此节点的子节点列表的前面。 |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | 将节点添加到此节点的子节点列表的末尾。 |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 按节点类型获取所有子节点。 |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | 将节点插入到此节点的子节点列表中的指定位置。 |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | 移除子节点。 |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [getFirstChild()](#getFirstChild--) | 获取此节点的第一个子节点。 |
| [getLastChild()](#getLastChild--) | 获取此节点的最后一个子节点。 |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | 从指定位置开始，将节点序列插入此节点的子节点列表中。 |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | 从指定位置开始，将节点序列插入此节点的子节点列表中。 |
| [isComposite()](#isComposite--) | 检查节点是否为复合节点。 |
| [iterator()](#iterator--) | 返回一个枚举器，用于遍历 `CompositeNode\{T\}` 的子节点。 |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


将节点添加到此节点的子节点列表的前面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newChild | T1 | 要添加的节点。 |

**Returns:**
T1 - 添加的节点。
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


将节点添加到此节点的子节点列表的末尾。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newChild | T1 | 要添加的节点。 |

**Returns:**
T1 - 添加的节点。
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


按节点类型获取所有子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 子节点的列表。

`T1`：返回列表中元素的类型。
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


将节点插入到此节点的子节点列表中的指定位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 插入位置 |
| newChild | T1 | 要插入的节点。 |

**Returns:**
T1 - 添加的节点。
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


移除子节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldChild | T1 | 要删除的节点。 |

**Returns:**
T1 - 被移除的节点。
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


获取此节点的第一个子节点。

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


获取此节点的最后一个子节点。

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


从指定位置开始，将节点序列插入此节点的子节点列表中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 插入位置 |
| newChildren | T[] | 要插入的节点序列。 |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


从指定位置开始，将节点序列插入此节点的子节点列表中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 插入位置 |
| newChildren | java.lang.Iterable&lt;T&gt; | 要插入的节点序列。 |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


检查节点是否为复合节点。如果为 true，则该节点可以拥有子节点。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


返回一个枚举器，用于遍历 `CompositeNode\{T\}` 的子节点。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - 用于 `CompositeNode\{T\}` 的 `T:IEnumerator`1`。
