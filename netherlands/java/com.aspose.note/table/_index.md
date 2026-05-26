---
title: "Table"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een tabel voor."
type: docs
weight: 87
url: /nl/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Stelt een tabel voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Table()](#Table--) | Initialiseert een nieuw exemplaar van de `Table`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getColumns()](#getColumns--) | Haalt de kolommen van de tabel op. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getTags()](#getTags--) | Haalt de lijst met alle tags van een tabel op. |
| [isBordersVisible()](#isBordersVisible--) | Haalt een waarde op die aangeeft of de tabelrand zichtbaar is. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Stelt een waarde in die aangeeft of de tabelrand zichtbaar is. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
### Table() {#Table--}
```
public Table()
```


Initialiseert een nieuw exemplaar van de `Table`-klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Haalt de kolommen van de tabel op.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Haalt de lijst met alle tags van een tabel op.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Haalt een waarde op die aangeeft of de tabelrand zichtbaar is.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Stelt een waarde in die aangeeft of de tabelrand zichtbaar is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

