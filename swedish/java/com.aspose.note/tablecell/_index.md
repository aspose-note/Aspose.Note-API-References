---
title: "TableCell"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en tabellcell."
type: docs
weight: 88
url: /sv/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Representerar en tabellcell.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TableCell()](#TableCell--) | Initierar en ny instans av klassen `TableCell`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getBackgroundColor()](#getBackgroundColor--) | Hämtar bakgrundsfärgen. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getMaxWidth()](#getMaxWidth--) | Hämtar maximal bredd. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Ställer in bakgrundsfärgen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Initierar en ny instans av klassen `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Hämtar bakgrundsfärgen.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Hämtar antalet objekt som ska summeras i RgOutlineIndentDistance-arrayen för att få indragningsstorlek.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Hämtar maximal bredd.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Ställer in bakgrundsfärgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

