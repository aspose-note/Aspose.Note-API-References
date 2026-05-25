---
title: "CompositeNode"
second_title: "Riferimento API di Aspose.Note per Java"
description: "La classe generica di base per i nodi che possono contenere altri nodi."
type: docs
weight: 15
url: /it/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

La classe generica di base per i nodi che possono contenere altri nodi.

`T`: Il tipo di elementi nel nodo composito.

T :
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Aggiunge il nodo all'inizio dell'elenco dei nodi figlio per questo nodo. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Aggiunge il nodo alla fine dell'elenco dei nodi figlio per questo nodo. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ottieni tutti i nodi figli per tipo di nodo. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Inserisce il nodo nella posizione specificata nell'elenco dei nodi figlio per questo nodo. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Rimuove il nodo figlio. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getFirstChild()](#getFirstChild--) | Ottiene il primo nodo figlio di questo nodo. |
| [getLastChild()](#getLastChild--) | Ottiene l'ultimo nodo figlio di questo nodo. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Inserisce la sequenza del nodo a partire dalla posizione specificata nell'elenco dei nodi figlio per questo nodo. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Inserisce la sequenza del nodo a partire dalla posizione specificata nell'elenco dei nodi figlio per questo nodo. |
| [isComposite()](#isComposite--) | Verifica se il nodo è composito. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso i nodi figlio del `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Aggiunge il nodo all'inizio dell'elenco dei nodi figlio per questo nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newChild | T1 | Il nodo da aggiungere. |

**Returns:**
T1 - Il nodo aggiunto.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Aggiunge il nodo alla fine dell'elenco dei nodi figlio per questo nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newChild | T1 | Il nodo da aggiungere. |

**Returns:**
T1 - Il nodo aggiunto.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ottieni tutti i nodi figli per tipo di nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Un elenco di nodi figli.

`T1`: Il tipo di elementi nella lista restituita.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Inserisce il nodo nella posizione specificata nell'elenco dei nodi figlio per questo nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | Posizione in cui inserire |
| newChild | T1 | Il nodo da inserire. |

**Returns:**
T1 - Il nodo aggiunto.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Rimuove il nodo figlio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldChild | T1 | Il nodo da rimuovere. |

**Returns:**
T1 - Il nodo rimosso.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Ottiene il primo nodo figlio di questo nodo.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Ottiene l'ultimo nodo figlio di questo nodo.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Inserisce la sequenza del nodo a partire dalla posizione specificata nell'elenco dei nodi figlio per questo nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | Posizione in cui inserire |
| newChildren | T[] | La sequenza di nodi da inserire. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Inserisce la sequenza del nodo a partire dalla posizione specificata nell'elenco dei nodi figlio per questo nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| i | int | Posizione in cui inserire |
| newChildren | java.lang.Iterable&lt;T&gt; | La sequenza di nodi da inserire. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Verifica se il nodo è composito. Se vero, il nodo può avere nodi figli.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Restituisce un enumeratore che itera attraverso i nodi figlio del `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Un `T:IEnumerator`1` per il `CompositeNode\{T\}`.
