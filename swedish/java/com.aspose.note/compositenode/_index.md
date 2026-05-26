---
title: "CompositeNode"
second_title: "Aspose.Note for Java API-referens"
description: "Den grundläggande generiska klassen för noder som kan innehålla andra noder."
type: docs
weight: 15
url: /sv/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Den grundläggande generiska klassen för noder som kan innehålla andra noder.

`T`: Typen av element i den sammansatta noden.

T :
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Lägger till noden i början av listan med underordnade noder för den här noden. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Lägger till noden i slutet av listan med underordnade noder för den här noden. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Hämta alla underordnade noder efter nodtypen. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Infogar noden på den angivna positionen i listan med underordnade noder för den här noden. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Tar bort den underordnade noden. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getFirstChild()](#getFirstChild--) | Hämtar den första underordnade noden för den här noden. |
| [getLastChild()](#getLastChild--) | Hämtar den sista underordnade noden för den här noden. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Infogar nodens sekvens med start från angiven position i listan med underordnade noder för den här noden. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Infogar nodens sekvens med start från angiven position i listan med underordnade noder för den här noden. |
| [isComposite()](#isComposite--) | Kontrollerar om noden är sammansatt. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom underordnade noder för `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Lägger till noden i början av listan med underordnade noder för den här noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newChild | T1 | Noden att lägga till. |

**Returns:**
T1 - Den tillagda noden.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Lägger till noden i slutet av listan med underordnade noder för den här noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newChild | T1 | Noden att lägga till. |

**Returns:**
T1 - Den tillagda noden.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Hämta alla underordnade noder efter nodtypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - En lista med barnnoder.

`T1`: Typen av element i den returnerade listan.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Infogar noden på den angivna positionen i listan med underordnade noder för den här noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| i | int | Position att infoga |
| newChild | T1 | Noden att infoga. |

**Returns:**
T1 - Den tillagda noden.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Tar bort den underordnade noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| oldChild | T1 | Noden att ta bort. |

**Returns:**
T1 - Den borttagna noden.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Hämtar den första underordnade noden för den här noden.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Hämtar den sista underordnade noden för den här noden.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Infogar nodens sekvens med start från angiven position i listan med underordnade noder för den här noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| i | int | Position att infoga |
| newChildren | T[] | Sekvensen av noder som ska infogas. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Infogar nodens sekvens med start från angiven position i listan med underordnade noder för den här noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| i | int | Position att infoga |
| newChildren | java.lang.Iterable&lt;T&gt; | Sekvensen av noder som ska infogas. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Kontrollerar om noden är sammansatt. Om true kan noden ha barnnoder.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Returnerar en enumerator som itererar genom underordnade noder för `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - En `T:IEnumerator`1` för `CompositeNode\{T\}`.
