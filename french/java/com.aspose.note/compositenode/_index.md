---
title: "CompositeNode"
second_title: "Référence d'API Aspose.Note pour Java"
description: "La classe générique de base pour les nœuds pouvant contenir d'autres nœuds."
type: docs
weight: 15
url: /fr/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

La classe générique de base pour les nœuds pouvant contenir d'autres nœuds.

`T`: Le type des éléments dans le nœud composite.

T :
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Ajoute le nœud au début de la liste des nœuds enfants de ce nœud. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Ajoute le nœud à la fin de la liste des nœuds enfants de ce nœud. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtient tous les nœuds enfants par type de nœud. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Insère le nœud à la position spécifiée dans la liste des nœuds enfants de ce nœud. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Supprime le nœud enfant. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getFirstChild()](#getFirstChild--) | Obtient le premier nœud enfant de ce nœud. |
| [getLastChild()](#getLastChild--) | Obtient le dernier nœud enfant de ce nœud. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Insère la séquence du nœud à partir de la position spécifiée dans la liste des nœuds enfants de ce nœud. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Insère la séquence du nœud à partir de la position spécifiée dans la liste des nœuds enfants de ce nœud. |
| [isComposite()](#isComposite--) | Vérifie si le nœud est composite. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt les nœuds enfants du `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Ajoute le nœud au début de la liste des nœuds enfants de ce nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newChild | T1 | Le nœud à ajouter. |

**Returns:**
T1 - Le nœud ajouté.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Ajoute le nœud à la fin de la liste des nœuds enfants de ce nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newChild | T1 | Le nœud à ajouter. |

**Returns:**
T1 - Le nœud ajouté.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtient tous les nœuds enfants par type de nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Une liste de nœuds enfants.

`T1`: Le type des éléments dans la liste retournée.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Insère le nœud à la position spécifiée dans la liste des nœuds enfants de ce nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | Position d'insertion |
| newChild | T1 | Le nœud à insérer. |

**Returns:**
T1 - Le nœud ajouté.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Supprime le nœud enfant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| oldChild | T1 | Le nœud à supprimer. |

**Returns:**
T1 - Le nœud supprimé.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Obtient le premier nœud enfant de ce nœud.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Obtient le dernier nœud enfant de ce nœud.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Insère la séquence du nœud à partir de la position spécifiée dans la liste des nœuds enfants de ce nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | Position d'insertion |
| newChildren | T[] | La séquence de nœuds à insérer. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Insère la séquence du nœud à partir de la position spécifiée dans la liste des nœuds enfants de ce nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | Position d'insertion |
| newChildren | java.lang.Iterable&lt;T&gt; | La séquence de nœuds à insérer. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Vérifie si le nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Renvoie un énumérateur qui parcourt les nœuds enfants du `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Un `T:IEnumerator`1` pour le `CompositeNode\{T\}`.
