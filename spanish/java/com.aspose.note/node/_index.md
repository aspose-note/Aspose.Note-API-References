---
title: "Nodo"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La clase base para todos los nodos de un documento Aspose.Note."
type: docs
weight: 51
url: /es/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

La clase base para todos los nodos de un documento Aspose.Note.
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getDocument()](#getDocument--) | Obtiene el documento del nodo. |
| [getNextSibling()](#getNextSibling--) | Obtiene el nodo siguiente en el mismo nivel del árbol de nodos. |
| [getNodeId()](#getNodeId--) | Obtiene el ID del nodo. |
| [getNodeType()](#getNodeType--) | Obtiene el tipo de nodo. |
| [getParentNode()](#getParentNode--) | Obtiene el nodo padre. |
| [getPreviousSibling()](#getPreviousSibling--) | Obtiene el nodo anterior en el mismo nivel del árbol de nodos. |
| [isComposite()](#isComposite--) | Obtiene un valor que indica si este nodo es compuesto. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Obtiene el documento del nodo.

Valor: El documento.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Obtiene el nodo siguiente en el mismo nivel del árbol de nodos.

Valor: El siguiente hermano.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Obtiene el ID del nodo.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Obtiene el tipo de nodo.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Obtiene el nodo padre.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Obtiene el nodo anterior en el mismo nivel del árbol de nodos.

Valor: El hermano anterior.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Obtiene un valor que indica si este nodo es compuesto. Si es verdadero, el nodo puede tener nodos hijos.

**Returns:**
boolean
