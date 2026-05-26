---
title: "CompositeNode"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La clase genérica base para nodos que pueden contener otros nodos."
type: docs
weight: 15
url: /es/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

La clase genérica base para nodos que pueden contener otros nodos.

`T`: El tipo de elementos en el nodo compuesto.

T :
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Agrega el nodo al principio de la lista de nodos hijos de este nodo. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Agrega el nodo al final de la lista de nodos hijos de este nodo. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtiene todos los nodos hijos por el tipo de nodo. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserta el nodo en la posición especificada de la lista de nodos hijos de este nodo. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Elimina el nodo hijo. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getFirstChild()](#getFirstChild--) | Obtiene el primer nodo hijo de este nodo. |
| [getLastChild()](#getLastChild--) | Obtiene el último nodo hijo de este nodo. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserta la secuencia del nodo comenzando desde la posición especificada en la lista de nodos hijos de este nodo. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserta la secuencia del nodo comenzando desde la posición especificada en la lista de nodos hijos de este nodo. |
| [isComposite()](#isComposite--) | Comprueba si el nodo es compuesto. |
| [iterator()](#iterator--) | Devuelve un enumerador que itera a través de los nodos hijos del `CompositeNode\\{T\\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Agrega el nodo al principio de la lista de nodos hijos de este nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newChild | T1 | El nodo a agregar. |

**Returns:**
T1 - El nodo agregado.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Agrega el nodo al final de la lista de nodos hijos de este nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newChild | T1 | El nodo a agregar. |

**Returns:**
T1 - El nodo agregado.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtiene todos los nodos hijos por el tipo de nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Una lista de nodos hijos.

`T1`: El tipo de elementos en la lista devuelta.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Inserta el nodo en la posición especificada de la lista de nodos hijos de este nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| i | int | Posición para insertar |
| newChild | T1 | El nodo a insertar. |

**Returns:**
T1 - El nodo agregado.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Elimina el nodo hijo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| oldChild | T1 | El nodo a eliminar. |

**Returns:**
T1 - El nodo eliminado.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Obtiene el primer nodo hijo de este nodo.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Obtiene el último nodo hijo de este nodo.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Inserta la secuencia del nodo comenzando desde la posición especificada en la lista de nodos hijos de este nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| i | int | Posición para insertar |
| newChildren | T[] | La secuencia de nodos a insertar. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Inserta la secuencia del nodo comenzando desde la posición especificada en la lista de nodos hijos de este nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| i | int | Posición para insertar |
| newChildren | java.lang.Iterable&lt;T&gt; | La secuencia de nodos a insertar. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Comprueba si el nodo es compuesto. Si es verdadero, entonces el nodo puede tener nodos hijos.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Devuelve un enumerador que itera a través de los nodos hijos del `CompositeNode\\{T\\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Un `T:IEnumerator`1` para el `CompositeNode\{T\}`.
