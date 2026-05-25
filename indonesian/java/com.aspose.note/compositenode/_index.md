---
title: "CompositeNode"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas generik dasar untuk node yang dapat berisi node lain."
type: docs
weight: 15
url: /id/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Kelas generik dasar untuk node yang dapat berisi node lain.

`T`: Tipe elemen dalam node komposit.

T :
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Menambahkan node ke depan daftar node anak untuk node ini. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Menambahkan node ke akhir daftar node anak untuk node ini. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Dapatkan semua node anak berdasarkan tipe node. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Menyisipkan node ke posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Menghapus node anak. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getFirstChild()](#getFirstChild--) | Mendapatkan node anak pertama dari node ini. |
| [getLastChild()](#getLastChild--) | Mendapatkan node anak terakhir dari node ini. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini. |
| [isComposite()](#isComposite--) | Memeriksa apakah node bersifat komposit. |
| [iterator()](#iterator--) | Mengembalikan enumerator yang mengiterasi node anak dari `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Menambahkan node ke depan daftar node anak untuk node ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newChild | T1 | Node yang akan ditambahkan. |

**Returns:**
T1 - Node yang ditambahkan.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Menambahkan node ke akhir daftar node anak untuk node ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newChild | T1 | Node yang akan ditambahkan. |

**Returns:**
T1 - Node yang ditambahkan.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Dapatkan semua node anak berdasarkan tipe node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Daftar node anak.

`T1`: Tipe elemen dalam daftar yang dikembalikan.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Menyisipkan node ke posisi yang ditentukan dalam daftar node anak untuk node ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| i | int | Posisi untuk menyisipkan |
| newChild | T1 | Node yang akan disisipkan. |

**Returns:**
T1 - Node yang ditambahkan.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Menghapus node anak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldChild | T1 | Node yang akan dihapus. |

**Returns:**
T1 - Node yang dihapus.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Mendapatkan node anak pertama dari node ini.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Mendapatkan node anak terakhir dari node ini.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| i | int | Posisi untuk menyisipkan |
| newChildren | T[] | Urutan node yang akan disisipkan. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Menyisipkan urutan node mulai dari posisi yang ditentukan dalam daftar node anak untuk node ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| i | int | Posisi untuk menyisipkan |
| newChildren | java.lang.Iterable&lt;T&gt; | Urutan node yang akan disisipkan. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Memeriksa apakah node bersifat komposit. Jika true maka node dapat memiliki node anak.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Mengembalikan enumerator yang mengiterasi node anak dari `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - Sebuah `T:IEnumerator`1` untuk `CompositeNode\{T\}`.
