---
title: Table
second_title: Aspose.Note for Java API Reference
description: Represents a table.
type: docs
weight: 87
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
| [Table()](#Table--) | Initializes a new instance of the `Table` class. |
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getColumns()](#getColumns--) | Gets the columns of the table. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Gets or sets the last modified time. |
| [getTags()](#getTags--) | Gets the list of all tags of a table. |
| [isBordersVisible()](#isBordersVisible--) | Gets a value indicating whether the table border is visible. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Sets a value indicating whether the table border is visible. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Gets or sets the last modified time. |
### Table() {#Table--}
```
public Table()
```


Initializes a new instance of the `Table` class.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Gets the columns of the table.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Gets or sets the last modified time.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Gets the list of all tags of a table.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
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

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Gets or sets the last modified time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

