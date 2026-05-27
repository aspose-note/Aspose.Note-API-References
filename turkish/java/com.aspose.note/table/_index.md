---
title: "Table"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir tabloyu temsil eder."
type: docs
weight: 87
url: /tr/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Bir tabloyu temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Table()](#Table--) | `Table` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getColumns()](#getColumns--) | Tablonun sütunlarını alır. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getTags()](#getTags--) | Bir tablonun tüm etiketlerinin listesini alır. |
| [isBordersVisible()](#isBordersVisible--) | Tablo kenarlığının görünür olup olmadığını gösteren bir değeri alır. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Tablo kenarlığının görünür olup olmadığını gösteren bir değeri ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
### Table() {#Table--}
```
public Table()
```


`Table` sınıfının yeni bir örneğini başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Tablonun sütunlarını alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Bir tablonun tüm etiketlerinin listesini alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Tablo kenarlığının görünür olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Tablo kenarlığının görünür olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

