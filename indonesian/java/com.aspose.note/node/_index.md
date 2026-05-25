---
title: "Node"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar untuk semua node dalam dokumen Aspose.Note."
type: docs
weight: 51
url: /id/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Kelas dasar untuk semua node dalam dokumen Aspose.Note.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getDocument()](#getDocument--) | Mendapatkan dokumen dari node. |
| [getNextSibling()](#getNextSibling--) | Mendapatkan node berikutnya pada tingkat pohon node yang sama. |
| [getNodeId()](#getNodeId--) | Mendapatkan ID node. |
| [getNodeType()](#getNodeType--) | Mendapatkan tipe node. |
| [getParentNode()](#getParentNode--) | Mendapatkan node induk. |
| [getPreviousSibling()](#getPreviousSibling--) | Mendapatkan node sebelumnya pada tingkat pohon node yang sama. |
| [isComposite()](#isComposite--) | Mendapatkan nilai yang menunjukkan apakah node ini komposit. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Mendapatkan dokumen dari node.

Nilai: Dokumen.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Mendapatkan node berikutnya pada tingkat pohon node yang sama.

Nilai: Saudara berikutnya.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Mendapatkan ID node.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Mendapatkan tipe node.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Mendapatkan node induk.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Mendapatkan node sebelumnya pada tingkat pohon node yang sama.

Nilai: Saudara sebelumnya.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Mendapatkan nilai yang menunjukkan apakah node ini komposit. Jika true, node dapat memiliki node anak.

**Returns:**
boolean
