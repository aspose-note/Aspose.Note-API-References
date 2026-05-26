---
title: "OutlineElement"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een OutlineElement voor."
type: docs
weight: 67
url: /nl/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Stelt een OutlineElement voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Initialiseert een nieuw exemplaar van de `OutlineElement`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Haalt de meest recente auteur van een outline-element op. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Haalt de oorspronkelijke auteur van een outline-element op. |
| [getCreationTime()](#getCreationTime--) | Haalt het aanmaaktijdstip op of stelt het in. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getNumberList()](#getNumberList--) | Haalt de stijl op of stelt de stijl in voor de kop van een genummerde lijst. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Haalt het aanmaaktijdstip op of stelt het in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Haalt de stijl op of stelt de stijl in voor de kop van een genummerde lijst. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initialiseert een nieuw exemplaar van de `OutlineElement`-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Haalt de meest recente auteur van een outline-element op.

Waarde: De meest recente auteur.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Haalt de oorspronkelijke auteur van een outline-element op.

Waarde: De oorspronkelijke auteur.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Haalt het aanmaaktijdstip op of stelt het in.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Haalt de stijl op of stelt de stijl in voor de kop van een genummerde lijst.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Haalt het aanmaaktijdstip op of stelt het in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Haalt de stijl op of stelt de stijl in voor de kop van een genummerde lijst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

