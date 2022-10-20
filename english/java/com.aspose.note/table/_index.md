---
title: Table
second_title: Aspose.Note for Java API Reference
description: Represents a table.
type: docs
weight: 71
url: /java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Represents a table.
## Constructors

| Constructor | Description |
| --- | --- |
| [Table(Document document)](#Table-com.aspose.note.Document-) | Initializes a new instance of the  Table  class. |
| [Table()](#Table--) | Initializes a new instance of the  Table  class. |
## Methods

| Method | Description |
| --- | --- |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
| [isBordersVisible()](#isBordersVisible--) | Gets a value indicating whether the table border is visible. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Sets a value indicating whether the table border is visible. |
| [getColumns()](#getColumns--) | Gets the columns of the table. |
| [getTags()](#getTags--) | Gets the list of all tags of a table. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
### Table(Document document) {#Table-com.aspose.note.Document-}
```
public Table(Document document)
```


Initializes a new instance of the  Table  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The parent document of the table. |

### Table() {#Table--}
```
public Table()
```


Initializes a new instance of the  Table  class.

### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Gets a value indicating whether the table border is visible.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Sets a value indicating whether the table border is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Gets the columns of the table.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList<com.aspose.note.TableColumn>
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of all tags of a table.

**Returns:**
com.aspose.ms.System.Collections.Generic.List<com.aspose.note.ITag>
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

