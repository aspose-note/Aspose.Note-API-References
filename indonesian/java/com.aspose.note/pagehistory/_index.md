---
title: "PageHistory"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili riwayat halaman."
type: docs
weight: 70
url: /id/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Mewakili riwayat halaman.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Menginisialisasi instance baru dari kelas `PageHistory`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Menambahkan versi halaman ke akhir `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Menambahkan versi-versi halaman ke akhir `PageHistory`. |
| [clear()](#clear--) | Menghapus riwayat halaman. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Menentukan apakah riwayat halaman berisi versi halaman. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Menyalin versi halaman ke dalam array, mulai pada indeks tertentu.. |
| [getCurrent()](#getCurrent--) | Mendapatkan versi halaman saat ini. |
| [get_Item(int index)](#get-Item-int-) | Mendapatkan atau mengatur versi halaman pada indeks yang ditentukan dari `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Menentukan indeks dari versi halaman tertentu dalam riwayat halaman. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Menyisipkan versi halaman ke dalam riwayat halaman. |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah riwayat halaman hanya baca. |
| [iterator()](#iterator--) | Mengembalikan enumerator yang mengiterasi node anak dari `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Menghapus versi halaman pada indeks yang ditentukan dari `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Menghapus versi halaman dari `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Menghapus rentang versi halaman dari `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Mendapatkan atau mengatur versi halaman pada indeks yang ditentukan dari `PageHistory`. |
| [size()](#size--) | Mendapatkan jumlah versi halaman dalam riwayat halaman. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Menginisialisasi instance baru dari kelas `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Versi halaman saat ini. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Menambahkan versi halaman ke akhir `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Versi halaman. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Menambahkan versi-versi halaman ke akhir `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Koleksi `IEnumerable\{Page\}` dari versi halaman. |

### clear() {#clear--}
```
public void clear()
```


Menghapus riwayat halaman.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Menentukan apakah riwayat halaman berisi versi halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Versi halaman. |

**Returns:**
boolean - `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Menyalin versi halaman ke dalam array, mulai pada indeks tertentu..

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Array target. |
| arrayIndex | int | Indeks array. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Mendapatkan versi halaman saat ini.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Mendapatkan atau mengatur versi halaman pada indeks yang ditentukan dari `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Menentukan indeks dari versi halaman tertentu dalam riwayat halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Versi halaman. |

**Returns:**
int - `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Menyisipkan versi halaman ke dalam riwayat halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks. |
| item | [Page](../../com.aspose.note/page) | Versi halaman. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah riwayat halaman hanya baca.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Mengembalikan enumerator yang mengiterasi node anak dari `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Menghapus versi halaman pada indeks yang ditentukan dari `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Menghapus versi halaman dari `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Versi halaman. |

**Returns:**
boolean - `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Menghapus rentang versi halaman dari `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks. |
| count | int | Jumlahnya. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Mendapatkan atau mengatur versi halaman pada indeks yang ditentukan dari `PageHistory`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Mendapatkan jumlah versi halaman dalam riwayat halaman.

**Returns:**
int
