---
title: "CompositeNode"
second_title: "Aspose.Note for Java API Referansı"
description: "Diğer düğümleri içerebilen düğümler için temel genel sınıf."
type: docs
weight: 15
url: /tr/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Diğer düğümleri içerebilen düğümler için temel genel sınıf.

`T`: Bileşik düğümdeki öğelerin türü.

T :
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Bu düğümün alt düğüm listesine düğümü listenin başına ekler. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Bu düğümün alt düğüm listesine düğümü listenin sonuna ekler. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Düğüm türüne göre tüm alt düğümleri al. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Bu düğümün alt düğüm listesinde belirtilen konuma düğümü ekler. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Alt düğümü kaldırır. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getFirstChild()](#getFirstChild--) | Bu düğümün ilk alt düğümünü alır. |
| [getLastChild()](#getLastChild--) | Bu düğümün son alt düğümünü alır. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Bu düğümün alt düğüm listesinde belirtilen konumdan başlayarak düğüm dizisini ekler. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Bu düğümün alt düğüm listesinde belirtilen konumdan başlayarak düğüm dizisini ekler. |
| [isComposite()](#isComposite--) | Düğümün birleşik olup olmadığını kontrol eder. |
| [iterator()](#iterator--) | `CompositeNode\{T\}` alt düğümleri arasında yineleme yapan bir enumerator döndürür. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Bu düğümün alt düğüm listesine düğümü listenin başına ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newChild | T1 | Eklenecek düğüm. |

**Returns:**
T1 - Eklenen düğüm.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Bu düğümün alt düğüm listesine düğümü listenin sonuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newChild | T1 | Eklenecek düğüm. |

**Returns:**
T1 - Eklenen düğüm.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Düğüm türüne göre tüm alt düğümleri al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Çocuk düğümlerin bir listesi.

`T1`: Döndürülen listedeki öğelerin tipi.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Bu düğümün alt düğüm listesinde belirtilen konuma düğümü ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | Eklenecek konum |
| newChild | T1 | Eklenecek düğüm. |

**Returns:**
T1 - Eklenen düğüm.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Alt düğümü kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldChild | T1 | Kaldırılacak düğüm. |

**Returns:**
T1 - Kaldırılan düğüm.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Bu düğümün ilk alt düğümünü alır.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Bu düğümün son alt düğümünü alır.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Bu düğümün alt düğüm listesinde belirtilen konumdan başlayarak düğüm dizisini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | Eklenecek konum |
| newChildren | T[] | Eklenecek düğüm dizisi. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Bu düğümün alt düğüm listesinde belirtilen konumdan başlayarak düğüm dizisini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | Eklenecek konum |
| newChildren | java.lang.Iterable&lt;T&gt; | Eklenecek düğüm dizisi. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Düğümün birleşik olup olmadığını kontrol eder. Doğruysa düğümün alt düğümleri olabilir.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


`CompositeNode\{T\}` alt düğümleri arasında yineleme yapan bir enumerator döndürür.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - `T:IEnumerator`1` için `CompositeNode\{T\}`.
