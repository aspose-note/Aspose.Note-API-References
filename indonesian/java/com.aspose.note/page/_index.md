---
title: "Page"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili sebuah halaman."
type: docs
weight: 69
url: /id/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Mewakili sebuah halaman.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Page()](#Page--) | Menginisialisasi instance baru dari kelas `Page`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [deepClone()](#deepClone--) | Menggandakan halaman. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Menggandakan halaman. |
| [getAuthor()](#getAuthor--) | Mendapatkan atau mengatur penulis. |
| [getBackgroundColor()](#getBackgroundColor--) | Mendapatkan atau mengatur warna latar belakang halaman. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan atau mengatur waktu pembuatan. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [getLevel()](#getLevel--) | Mendapatkan atau mengatur level. |
| [getMargin()](#getMargin--) | Mendapatkan atau mengatur margin. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Mendapatkan atau mengatur ringkasan revisi untuk halaman dan node anaknya. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Mendapatkan ukuran tata letak halaman yang ditampilkan di editor. |
| [getSizeType()](#getSizeType--) | Mendapatkan atau mengatur tipe ukuran sebuah halaman. |
| [getTitle()](#getTitle--) | Mendapatkan atau mengatur judul. |
| [isConflictPage()](#isConflictPage--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman ini adalah halaman konflik. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Mendapatkan atau mengatur penulis. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Mendapatkan atau mengatur warna latar belakang halaman. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman ini adalah halaman konflik. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Mendapatkan atau mengatur waktu pembuatan. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [setLevel(byte value)](#setLevel-byte-) | Mendapatkan atau mengatur level. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Mendapatkan atau mengatur margin. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Mendapatkan atau mengatur ringkasan revisi untuk halaman dan node anaknya. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Mengatur ukuran tata letak halaman yang ditampilkan di editor. |
| [setSizeType(int value)](#setSizeType-int-) | Mendapatkan atau mengatur tipe ukuran sebuah halaman. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Mendapatkan atau mengatur judul. |
### Page() {#Page--}
```
public Page()
```


Menginisialisasi instance baru dari kelas `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Menggandakan halaman.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Menggandakan halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| cloneHistory | boolean | Menentukan apakah riwayat halaman harus digandakan. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Mendapatkan atau mengatur penulis.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Mendapatkan atau mengatur warna latar belakang halaman.

**Returns:**
java.awt.Color
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
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Mendapatkan atau mengatur level.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Mendapatkan atau mengatur margin.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Mendapatkan atau mengatur ringkasan revisi untuk halaman dan node anaknya.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Mendapatkan ukuran tata letak halaman yang ditampilkan di editor.

--------------------

Nilai ini digunakan oleh aplikasi Microsoft OneNote untuk menampilkan tata letak halaman dasar saat dokumen dibuka. Nilai ini tidak memengaruhi pencetakan dan penyimpanan dokumen. Ketika properti Page.SizeType diatur ke PageSizeType.SizeByContent, properti ini mengembalikan ukuran sebenarnya dari konten.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Mendapatkan atau mengatur tipe ukuran sebuah halaman.

--------------------

Secara default, halaman secara otomatis mengubah ukuran. Nilai default adalah [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Mendapatkan atau mengatur judul.

Nilai: `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman ini adalah halaman konflik.

--------------------

Halaman konflik muncul ketika dua pengguna mencoba memperbarui konten yang sama. Dalam kasus ini, perubahan pengguna pertama ditulis seperti biasa. Namun perubahan pengguna lain tidak dapat digabungkan. Jadi hanya salinan halaman yang dibuat dan ditandai sebagai konflik.

Pada versi ini, konflik diselesaikan dengan mengutamakan perubahan pengguna pertama. Jadi jika dokumen memiliki halaman konflik, halaman tersebut akan ditampilkan dalam riwayat tetapi akan dilewati saat penyimpanan. Flag ini dapat direset untuk menyimpan halaman tersebut dalam riwayat seperti halaman biasa.

Contoh detail tentang manipulasi halaman konflik dapat ditemukan di dokumentasi online.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Mendapatkan atau mengatur penulis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Mendapatkan atau mengatur warna latar belakang halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah halaman ini adalah halaman konflik.

--------------------

Halaman konflik muncul ketika dua pengguna mencoba memperbarui konten yang sama. Dalam kasus ini, perubahan pengguna pertama ditulis seperti biasa. Namun perubahan pengguna lain tidak dapat digabungkan. Jadi hanya salinan halaman yang dibuat dan ditandai sebagai konflik.

Pada versi ini, konflik diselesaikan dengan mengutamakan perubahan pengguna pertama. Jadi jika dokumen memiliki halaman konflik, halaman tersebut akan ditampilkan dalam riwayat tetapi akan dilewati saat penyimpanan. Flag ini dapat direset untuk menyimpan halaman tersebut dalam riwayat seperti halaman biasa.

Contoh detail tentang manipulasi halaman konflik dapat ditemukan di dokumentasi online.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

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

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Mendapatkan atau mengatur level.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Mendapatkan atau mengatur margin.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Mendapatkan atau mengatur ringkasan revisi untuk halaman dan node anaknya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Mengatur ukuran tata letak halaman yang ditampilkan di editor.

--------------------

Nilai ini digunakan oleh aplikasi Microsoft OneNote untuk menampilkan tata letak halaman dasar saat dokumen dibuka. Nilai ini tidak memengaruhi pencetakan dan penyimpanan dokumen. Ketika properti Page.SizeType diatur ke PageSizeType.SizeByContent, properti ini mengembalikan ukuran sebenarnya dari konten.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Mendapatkan atau mengatur tipe ukuran sebuah halaman.

--------------------

Secara default, halaman secara otomatis mengubah ukuran. Nilai default adalah [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Mendapatkan atau mengatur judul.

Nilai: `Title`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

