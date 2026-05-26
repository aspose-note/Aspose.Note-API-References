---
title: "Node"
second_title: "Aspose.Note for Java API-referentie"
description: "De basisklasse voor alle knooppunten van een Aspose.Note-document."
type: docs
weight: 51
url: /nl/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

De basisklasse voor alle knooppunten van een Aspose.Note-document.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getDocument()](#getDocument--) | Haalt het document van de node op. |
| [getNextSibling()](#getNextSibling--) | Haalt de volgende node op op hetzelfde node-boomniveau. |
| [getNodeId()](#getNodeId--) | Haalt de ID van de node op. |
| [getNodeType()](#getNodeType--) | Haalt het node-type op. |
| [getParentNode()](#getParentNode--) | Haalt de bovenliggende node op. |
| [getPreviousSibling()](#getPreviousSibling--) | Haalt de vorige node op op hetzelfde node-boomniveau. |
| [isComposite()](#isComposite--) | Haalt een waarde op die aangeeft of dit knooppunt samengesteld is. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Haalt het document van de node op.

Waarde: Het document.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Haalt de volgende node op op hetzelfde node-boomniveau.

Waarde: De volgende sibling.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Haalt de ID van de node op.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Haalt het node-type op.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Haalt de bovenliggende node op.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Haalt de vorige node op op hetzelfde node-boomniveau.

Waarde: De vorige sibling.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Haalt een waarde op die aangeeft of dit knooppunt samengesteld is. Indien waar kan het knooppunt onderliggende knooppunten hebben.

**Returns:**
boolean
