---
title: "Nod"
second_title: "Aspose.Note for Java API-referens"
description: "Bas-klassen för alla noder i ett **Aspose.Note**-dokument."
type: docs
weight: 51
url: /sv/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Bas-klassen för alla noder i ett **Aspose.Note**-dokument.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getDocument()](#getDocument--) | Hämtar nodens dokument. |
| [getNextSibling()](#getNextSibling--) | Hämtar nästa nod på samma nodträdnivå. |
| [getNodeId()](#getNodeId--) | Hämtar nodens ID. |
| [getNodeType()](#getNodeType--) | Hämtar nodtypen. |
| [getParentNode()](#getParentNode--) | Hämtar föräldranoden. |
| [getPreviousSibling()](#getPreviousSibling--) | Hämtar föregående nod på samma nodträdnivå. |
| [isComposite()](#isComposite--) | Hämtar ett värde som indikerar om denna nod är sammansatt. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Hämtar nodens dokument.

Värde: Dokumentet.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Hämtar nästa nod på samma nodträdnivå.

Värde: Nästa syskon.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Hämtar nodens ID.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Hämtar nodtypen.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Hämtar föräldranoden.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Hämtar föregående nod på samma nodträdnivå.

Värde: Föregående syskon.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Hämtar ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha undernoder.

**Returns:**
boolean
