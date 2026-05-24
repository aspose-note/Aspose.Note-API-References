---
title: "CompositeNode"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die generische Basisklasse für Knoten, die andere Knoten enthalten können."
type: docs
weight: 15
url: /de/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Die generische Basisklasse für Knoten, die andere Knoten enthalten können.

`T`: Der Typ der Elemente im zusammengesetzten Knoten.

T :
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Fügt den Knoten am Anfang der Liste von Kindknoten dieses Knotens hinzu. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Fügt den Knoten am Ende der Liste von Kindknoten dieses Knotens hinzu. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ruft alle untergeordneten Knoten nach Knotentyp ab. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Fügt den Knoten an der angegebenen Position in die Liste von Kindknoten dieses Knotens ein. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Entfernt den untergeordneten Knoten. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getFirstChild()](#getFirstChild--) | Gibt den ersten Kindknoten dieses Knotens zurück. |
| [getLastChild()](#getLastChild--) | Gibt den letzten Kindknoten dieses Knotens zurück. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste von Kindknoten dieses Knotens ein. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste von Kindknoten dieses Knotens ein. |
| [isComposite()](#isComposite--) | Überprüft, ob der Knoten zusammengesetzt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der durch die Kindknoten des `CompositeNode\{T\}` iteriert. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Fügt den Knoten am Anfang der Liste von Kindknoten dieses Knotens hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newChild | T1 | Der Knoten zum Hinzufügen. |

**Returns:**
T1 - Der hinzugefügte Knoten.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Fügt den Knoten am Ende der Liste von Kindknoten dieses Knotens hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newChild | T1 | Der Knoten zum Hinzufügen. |

**Returns:**
T1 - Der hinzugefügte Knoten.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ruft alle untergeordneten Knoten nach Knotentyp ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Eine Liste von Kindknoten.

`T1`: Der Typ der Elemente in der zurückgegebenen Liste.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Fügt den Knoten an der angegebenen Position in die Liste von Kindknoten dieses Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| i | int | Einfügeposition |
| newChild | T1 | Der einzufügende Knoten. |

**Returns:**
T1 - Der hinzugefügte Knoten.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Entfernt den untergeordneten Knoten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldChild | T1 | Der Knoten zum Entfernen. |

**Returns:**
T1 - Der entfernte Knoten.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Gibt den ersten Kindknoten dieses Knotens zurück.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Gibt den letzten Kindknoten dieses Knotens zurück.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste von Kindknoten dieses Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| i | int | Einfügeposition |
| newChildren | T[] | Die einzufügende Sequenz von Knoten. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste von Kindknoten dieses Knotens ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| i | int | Einfügeposition |
| newChildren | java.lang.Iterable&lt;T&gt; | Die einzufügende Sequenz von Knoten. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Überprüft, ob der Knoten zusammengesetzt ist. Wenn ja, kann der Knoten Kindknoten haben.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Gibt einen Enumerator zurück, der durch die Kindknoten des `CompositeNode\{T\}` iteriert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Ein `T:IEnumerator`1` für das `CompositeNode\{T\}`.
