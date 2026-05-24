---
title: "Nœud"
second_title: "Référence d'API Aspose.Note pour Java"
description: "La classe de base pour tous les nœuds d'un document Aspose.Note."
type: docs
weight: 51
url: /fr/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

La classe de base pour tous les nœuds d'un document Aspose.Note.
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getDocument()](#getDocument--) | Obtient le document du nœud. |
| [getNextSibling()](#getNextSibling--) | Obtient le nœud suivant au même niveau de l'arbre de nœuds. |
| [getNodeId()](#getNodeId--) | Obtient l'ID du nœud. |
| [getNodeType()](#getNodeType--) | Obtient le type de nœud. |
| [getParentNode()](#getParentNode--) | Obtient le nœud parent. |
| [getPreviousSibling()](#getPreviousSibling--) | Obtient le nœud précédent au même niveau de l'arbre de nœuds. |
| [isComposite()](#isComposite--) | Obtient une valeur indiquant si ce nœud est composite. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Obtient le document du nœud.

Value: le document.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Obtient le nœud suivant au même niveau de l'arbre de nœuds.

Value: le frère suivant.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Obtient l'ID du nœud.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Obtient le type de nœud.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Obtient le nœud parent.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Obtient le nœud précédent au même niveau de l'arbre de nœuds.

Value: le frère précédent.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants.

**Returns:**
boolean
