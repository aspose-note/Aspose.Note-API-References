---
title: "Nodo"
second_title: "Riferimento API di Aspose.Note per Java"
description: "La classe base per tutti i nodi di un documento Aspose.Note."
type: docs
weight: 51
url: /it/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

La classe base per tutti i nodi di un documento Aspose.Note.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getDocument()](#getDocument--) | Ottiene il documento del nodo. |
| [getNextSibling()](#getNextSibling--) | Ottiene il nodo successivo allo stesso livello dell'albero dei nodi. |
| [getNodeId()](#getNodeId--) | Ottiene l'ID del nodo. |
| [getNodeType()](#getNodeType--) | Ottiene il tipo di nodo. |
| [getParentNode()](#getParentNode--) | Ottiene il nodo genitore. |
| [getPreviousSibling()](#getPreviousSibling--) | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |
| [isComposite()](#isComposite--) | Ottiene un valore che indica se questo nodo è composito. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Ottiene il documento del nodo.

Valore: Il documento.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Ottiene il nodo successivo allo stesso livello dell'albero dei nodi.

Valore: Il fratello successivo.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Ottiene l'ID del nodo.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Ottiene il tipo di nodo.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Ottiene il nodo genitore.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Ottiene il nodo precedente allo stesso livello dell'albero dei nodi.

Valore: Il fratello precedente.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Ottiene un valore che indica se questo nodo è composito. Se vero, il nodo può avere nodi figli.

**Returns:**
boolean
