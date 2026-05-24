---
title: "Table"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل جدولًا."
type: docs
weight: 87
url: /ar/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

يمثل جدولًا.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Table()](#Table--) | ينشئ مثيلًا جديدًا من الفئة `Table`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getColumns()](#getColumns--) | يحصل على أعمدة الجدول. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getTags()](#getTags--) | يحصل على قائمة بجميع العلامات في جدول. |
| [isBordersVisible()](#isBordersVisible--) | يحصل على قيمة تشير إلى ما إذا كان حد الجدول مرئيًا. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كان حد الجدول مرئيًا. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
### Table() {#Table--}
```
public Table()
```


ينشئ مثيلًا جديدًا من الفئة `Table`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


يحصل على أعمدة الجدول.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل أو يضبط وقت التعديل الأخير.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


يحصل على قائمة بجميع العلامات في جدول.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


يحصل على قيمة تشير إلى ما إذا كان حد الجدول مرئيًا.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان حد الجدول مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

