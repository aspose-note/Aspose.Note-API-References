---
title: "Table"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili sebuah tabel."
type: docs
weight: 87
url: /id/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Mewakili sebuah tabel.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Table()](#Table--) | Menginisialisasi instance baru dari kelas `Table`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getColumns()](#getColumns--) | Mendapatkan kolom-kolom tabel. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [getTags()](#getTags--) | Mendapatkan daftar semua tag dari sebuah tabel. |
| [isBordersVisible()](#isBordersVisible--) | Mendapatkan nilai yang menunjukkan apakah batas tabel terlihat. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Mengatur nilai yang menunjukkan apakah batas tabel terlihat. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
### Table() {#Table--}
```
public Table()
```


Menginisialisasi instance baru dari kelas `Table`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Mendapatkan kolom-kolom tabel.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Mendapatkan daftar semua tag dari sebuah tabel.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Mendapatkan nilai yang menunjukkan apakah batas tabel terlihat.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Mengatur nilai yang menunjukkan apakah batas tabel terlihat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

