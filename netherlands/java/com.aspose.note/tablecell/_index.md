---
title: "TableCell"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een tabelcel voor."
type: docs
weight: 88
url: /nl/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Stelt een tabelcel voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TableCell()](#TableCell--) | Initialiseert een nieuw exemplaar van de `TableCell`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getBackgroundColor()](#getBackgroundColor--) | Haalt de achtergrondkleur op. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getMaxWidth()](#getMaxWidth--) | Haalt de maximale breedte op. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Stelt de achtergrondkleur in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Initialiseert een nieuw exemplaar van de `TableCell`-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Haalt de achtergrondkleur op.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Haalt de hoeveelheid items op die opgeteld moeten worden in de RgOutlineIndentDistance-array om de inspronggrootte te verkrijgen.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Haalt de maximale breedte op.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Stelt de achtergrondkleur in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

