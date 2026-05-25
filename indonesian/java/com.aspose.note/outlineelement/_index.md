---
title: "OutlineElement"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili sebuah OutlineElement."
type: docs
weight: 67
url: /id/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Mewakili sebuah OutlineElement.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Menginisialisasi instance baru dari kelas `OutlineElement`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Mendapatkan penulis terbaru dari elemen outline. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Mendapatkan penulis asli dari elemen outline. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan atau mengatur waktu pembuatan. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [getNumberList()](#getNumberList--) | Mendapatkan atau mengatur gaya untuk header daftar bernomor. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Mendapatkan atau mengatur waktu pembuatan. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Mendapatkan atau mengatur gaya untuk header daftar bernomor. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Menginisialisasi instance baru dari kelas `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Mendapatkan penulis terbaru dari elemen outline.

Nilai: Penulis terbaru.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Mendapatkan penulis asli dari elemen outline.

Nilai: Penulis asli.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Mendapatkan atau mengatur waktu pembuatan.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Mendapatkan atau mengatur gaya untuk header daftar bernomor.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Mendapatkan atau mengatur waktu pembuatan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Mendapatkan atau mengatur gaya untuk header daftar bernomor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

