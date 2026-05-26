---
title: "CompositeNode"
second_title: "Aspose.Note for Java API-referentie"
description: "De basisgenerieke klasse voor knooppunten die andere knooppunten kunnen bevatten."
type: docs
weight: 15
url: /nl/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

De basisgenerieke klasse voor knooppunten die andere knooppunten kunnen bevatten.

`T`: Het type elementen in het samengestelde knooppunt.

T :
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Voegt het knooppunt toe aan het begin van de lijst met onderliggende knooppunten voor dit knooppunt. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Voegt het knooppunt toe aan het einde van de lijst met onderliggende knooppunten voor dit knooppunt. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Haalt alle kindknopen op op basis van het knooptype. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Voegt het knooppunt in op de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Verwijdert de kindknoop. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getFirstChild()](#getFirstChild--) | Haalt het eerste onderliggende knooppunt van dit knooppunt op. |
| [getLastChild()](#getLastChild--) | Haalt het laatste onderliggende knooppunt van dit knooppunt op. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Voegt de reeks knooppunten in, beginnend vanaf de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Voegt de reeks knooppunten in, beginnend vanaf de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [isComposite()](#isComposite--) | Controleert of het knooppunt samengesteld is. |
| [iterator()](#iterator--) | Retourneert een enumerator die door de onderliggende knooppunten van de `CompositeNode\{T\}` itereren. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Voegt het knooppunt toe aan het begin van de lijst met onderliggende knooppunten voor dit knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newChild | T1 | Het toe te voegen knooppunt. |

**Returns:**
T1 - Het toegevoegde knooppunt.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Voegt het knooppunt toe aan het einde van de lijst met onderliggende knooppunten voor dit knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newChild | T1 | Het toe te voegen knooppunt. |

**Returns:**
T1 - Het toegevoegde knooppunt.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Haalt alle kindknopen op op basis van het knooptype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Een lijst van kindknooppunten.

`T1`: Het type van elementen in de geretourneerde lijst.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Voegt het knooppunt in op de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| i | int | Positie om in te voegen |
| newChild | T1 | Het knooppunt om in te voegen. |

**Returns:**
T1 - Het toegevoegde knooppunt.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Verwijdert de kindknoop.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| oldChild | T1 | Het te verwijderen knooppunt. |

**Returns:**
T1 - Het verwijderde knooppunt.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Haalt het eerste onderliggende knooppunt van dit knooppunt op.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Haalt het laatste onderliggende knooppunt van dit knooppunt op.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Voegt de reeks knooppunten in, beginnend vanaf de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| i | int | Positie om in te voegen |
| newChildren | T[] | De reeks knooppunten die ingevoegd moet worden. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Voegt de reeks knooppunten in, beginnend vanaf de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| i | int | Positie om in te voegen |
| newChildren | java.lang.Iterable&lt;T&gt; | De reeks knooppunten die ingevoegd moet worden. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Controleert of het knooppunt samengesteld is. Indien waar kan het knooppunt onderliggende knooppunten hebben.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Retourneert een enumerator die door de onderliggende knooppunten van de `CompositeNode\{T\}` itereren.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Een `T:IEnumerator`1` voor de `CompositeNode\{T\}`.
