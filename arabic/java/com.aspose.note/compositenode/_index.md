---
title: "CompositeNode"
second_title: "مرجع Aspose.Note for Java API"
description: "الفئة العامة الأساسية للعُقد التي يمكنها احتواء عُقد أخرى."
type: docs
weight: 15
url: /ar/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

الفئة العامة الأساسية للعُقد التي يمكنها احتواء عُقد أخرى.

`T`: نوع العناصر في العقدة المركبة.

T :
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | يضيف العقدة إلى بداية قائمة العقد الفرعية لهذا العقد. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | يضيف العقدة إلى نهاية قائمة العقد الفرعية لهذا العقد. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | احصل على جميع العقد الفرعية وفقًا لنوع العقدة. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | يدرج العقدة في الموضع المحدد في قائمة العقد الفرعية لهذا العقد. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | يزيل العقدة الفرعية. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getFirstChild()](#getFirstChild--) | يحصل على أول عقدة فرعية لهذا العقد. |
| [getLastChild()](#getLastChild--) | يحصل على آخر عقدة فرعية لهذا العقد. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | يدرج تسلسل العقد بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذا العقد. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | يدرج تسلسل العقد بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذا العقد. |
| [isComposite()](#isComposite--) | يتحقق مما إذا كانت العقدة مركبة. |
| [iterator()](#iterator--) | يرجع عدادًا يتنقل عبر العقد الفرعية لـ `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


يضيف العقدة إلى بداية قائمة العقد الفرعية لهذا العقد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| newChild | T1 | العقدة المراد إضافتها. |

**Returns:**
T1 - العقدة المضافة.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


يضيف العقدة إلى نهاية قائمة العقد الفرعية لهذا العقد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| newChild | T1 | العقدة المراد إضافتها. |

**Returns:**
T1 - العقدة المضافة.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


احصل على جميع العقد الفرعية وفقًا لنوع العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - قائمة بالعقد الفرعية.

`T1`: نوع العناصر في القائمة المعادة.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


يدرج العقدة في الموضع المحدد في قائمة العقد الفرعية لهذا العقد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | الموضع للإدراج |
| newChild | T1 | العقدة المراد إدراجها. |

**Returns:**
T1 - العقدة المضافة.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


يزيل العقدة الفرعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldChild | T1 | العقدة المراد إزالتها. |

**Returns:**
T1 - العقدة المُزالة.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


يحصل على أول عقدة فرعية لهذا العقد.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


يحصل على آخر عقدة فرعية لهذا العقد.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


يدرج تسلسل العقد بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذا العقد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | الموضع للإدراج |
| newChildren | T[] | تسلسل العقد المراد إدراجها. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


يدرج تسلسل العقد بدءًا من الموضع المحدد في قائمة العقد الفرعية لهذا العقد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | الموضع للإدراج |
| newChildren | java.lang.Iterable&lt;T&gt; | تسلسل العقد المراد إدراجها. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


يتحقق مما إذا كان العقدة مركبة. إذا كان صحيحًا فإن العقدة يمكن أن تحتوي على عقد فرعية.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


يرجع عدادًا يتنقل عبر العقد الفرعية لـ `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - أ `T:IEnumerator`1` لـ `CompositeNode\{T\}`.
