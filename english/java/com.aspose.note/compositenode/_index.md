---
title: CompositeNode
second_title: Aspose.Note for Java API Reference
description: The base generic class for nodes that can contain other nodes.
type: docs
weight: 15
url: /java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

The base generic class for nodes that can contain other nodes.

 T : The type of elements in the composite node.
## Methods

| Method | Description |
| --- | --- |
| [isComposite()](#isComposite--) | Checks whether the node is composite. |
| [getFirstChild()](#getFirstChild--) | Gets the first child node of this node. |
| [getLastChild()](#getLastChild--) | Gets the last child node of this node. |
| [getChildren()](#getChildren--) | Gets all child nodes of this node as an enumerable collection. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} . |
| [<T1>insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserts the node to the specified position in the list of child nodes for this node. |
| [insertChildrenRange(int i, Iterable<T> newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [<T1>appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Adds the node to the front of the list of child nodes for this node. |
| [<T1>appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Adds the node to the end of the list of child nodes for this node. |
| [<T1>removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Removes the child node. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Checks whether the node is composite. If true then the node can have child nodes.

**Returns:**
boolean
### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Gets the first child node of this node.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Gets the last child node of this node.

**Returns:**
T
### getChildren() {#getChildren--}
```
public List<T> getChildren()
```


Gets all child nodes of this node as an enumerable collection.

**Returns:**
java.util.List<T>
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Returns an enumerator that iterates through child nodes of the  CompositeNode\{T\} .

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<T> - A  T:IEnumerator1  for the  CompositeNode\{T\} .
### <T1>insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Inserts the node to the specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChild | T1 | The node to insert. |

**Returns:**
T1 - The added node.
### insertChildrenRange(int i, Iterable<T> newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Inserts the node's sequence starting from specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChildren | java.lang.Iterable<T> | The sequence of nodes to be inserted. |

### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Inserts the node's sequence starting from specified position in the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | int | Position to insert |
| newChildren | T[] | The sequence of nodes to be inserted. |

### <T1>appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Adds the node to the front of the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - The added node.
### <T1>appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Adds the node to the end of the list of child nodes for this node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | T1 | The node to add. |

**Returns:**
T1 - The added node.
### <T1>removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Removes the child node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChild | T1 | The node to remove. |

**Returns:**
T1 - The removed node.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

### <T1>getChildNodes(Class<T1> typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Get all child nodes by the node type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class<T1> |  |

**Returns:**
java.util.List<T1> - A list of child nodes.

 T1 : The type of elements in the returned list.
