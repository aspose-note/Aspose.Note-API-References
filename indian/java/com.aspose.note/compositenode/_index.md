---
title: "CompositeNode"
second_title: "Aspose.Note for Java API Reference"
description: "The base generic class for nodes that can contain other nodes."
type: docs
weight: 15
url: /hi/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

The base generic class for nodes that can contain other nodes.

`T`: The type of elements in the composite node.

T :
## Methods

| Method | Description |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | इस नोड के चाइल्ड नोड्स की सूची के सामने नोड को जोड़ता है. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | इस नोड के चाइल्ड नोड्स की सूची के अंत में नोड को जोड़ता है. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान पर नोड को सम्मिलित करता है. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Removes the child node. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getFirstChild()](#getFirstChild--) | इस नोड का पहला चाइल्ड नोड प्राप्त करता है. |
| [getLastChild()](#getLastChild--) | इस नोड का अंतिम चाइल्ड नोड प्राप्त करता है. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान से शुरू होकर नोड की क्रमबद्धता को सम्मिलित करता है. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान से शुरू होकर नोड की क्रमबद्धता को सम्मिलित करता है. |
| [isComposite()](#isComposite--) | जाँचता है कि नोड सम्मिश्र (कॉम्पोजिट) है या नहीं. |
| [iterator()](#iterator--) | `CompositeNode\{T\}` के चाइल्ड नोड्स के माध्यम से इटरैट करने वाला एनेमरेटर लौटाता है. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


इस नोड के चाइल्ड नोड्स की सूची के सामने नोड को जोड़ता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - जोड़ा गया नोड.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


इस नोड के चाइल्ड नोड्स की सूची के अंत में नोड को जोड़ता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - जोड़ा गया नोड.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Get all child nodes by the node type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - A list of child nodes.

`T1`: The type of elements in the returned list.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान पर नोड को सम्मिलित करता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | सम्मिलित करने का स्थान |
| newChild | T1 | सम्मिलित करने के लिए नोड. |

**Returns:**
T1 - जोड़ा गया नोड.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Removes the child node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChild | T1 | The node to remove. |

**Returns:**
T1 - हटाया गया नोड.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


इस नोड का पहला चाइल्ड नोड प्राप्त करता है.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


इस नोड का अंतिम चाइल्ड नोड प्राप्त करता है.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान से शुरू होकर नोड की क्रमबद्धता को सम्मिलित करता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | सम्मिलित करने का स्थान |
| newChildren | T[] | सम्मिलित किए जाने वाले नोड्स की क्रमबद्धता. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


इस नोड के चाइल्ड नोड्स की सूची में निर्दिष्ट स्थान से शुरू होकर नोड की क्रमबद्धता को सम्मिलित करता है.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | सम्मिलित करने का स्थान |
| newChildren | java.lang.Iterable&lt;T&gt; | सम्मिलित किए जाने वाले नोड्स की क्रमबद्धता. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


जाँचता है कि नोड संयुक्त है या नहीं। यदि सत्य है तो नोड के पास चाइल्ड नोड्स हो सकते हैं।

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


`CompositeNode\{T\}` के चाइल्ड नोड्स के माध्यम से इटरैट करने वाला एनेमरेटर लौटाता है.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - एक `T:IEnumerator`1` के लिए `CompositeNode\{T\}`.
