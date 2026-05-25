---
title: "IndentatedNode"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar untuk node dengan indentasi relatif bagi node anak."
type: docs
weight: 37
url: /id/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

Kelas dasar untuk node dengan indentasi relatif bagi node anak.

`T`: Tipe elemen dalam node komposit.

T :
Self :
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Mendapatkan atau mengatur posisi indentasi. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Mendapatkan jumlah item yang dijumlahkan dalam array RgOutlineIndentDistance untuk mendapatkan ukuran indentasi. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Mendapatkan atau mengatur posisi indentasi. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Mendapatkan atau mengatur posisi indentasi.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Mendapatkan jumlah item yang dijumlahkan dalam array RgOutlineIndentDistance untuk mendapatkan ukuran indentasi.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Mendapatkan atau mengatur posisi indentasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

**Returns:**
Self
