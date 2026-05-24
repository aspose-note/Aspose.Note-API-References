---
title: "Node"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die Basisklasse für alle Knoten eines Aspose.Note-Dokuments."
type: docs
weight: 51
url: /de/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Die Basisklasse für alle Knoten eines Aspose.Note-Dokuments.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getDocument()](#getDocument--) | Ruft das Dokument des Knotens ab. |
| [getNextSibling()](#getNextSibling--) | Ruft den nächsten Knoten auf derselben Baumebene ab. |
| [getNodeId()](#getNodeId--) | Ruft die ID des Knotens ab. |
| [getNodeType()](#getNodeType--) | Ruft den Knotentyp ab. |
| [getParentNode()](#getParentNode--) | Ruft den übergeordneten Knoten ab. |
| [getPreviousSibling()](#getPreviousSibling--) | Ruft den vorherigen Knoten auf derselben Baumebene ab. |
| [isComposite()](#isComposite--) | Ermittelt einen Wert, der angibt, ob dieser Knoten zusammengesetzt ist. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Ruft das Dokument des Knotens ab.

Wert: Das Dokument.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Ruft den nächsten Knoten auf derselben Baumebene ab.

Wert: Das nächste Geschwisterelement.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Ruft die ID des Knotens ab.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Ruft den Knotentyp ab.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Ruft den übergeordneten Knoten ab.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Ruft den vorherigen Knoten auf derselben Baumebene ab.

Wert: Das vorherige Geschwisterelement.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Ermittelt einen Wert, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn true, kann der Knoten Kindknoten haben.

**Returns:**
boolean
