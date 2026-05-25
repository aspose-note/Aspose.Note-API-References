---
title: "AttachedFile"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili file yang dilampirkan."
type: docs
weight: 11
url: /id/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Mewakili file yang dilampirkan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Menginisialisasi sebuah instance baru dari kelas `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Menginisialisasi sebuah instance baru dari kelas `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Menginisialisasi sebuah instance baru dari kelas `AttachedFile`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getAlignment()](#getAlignment--) | Mendapatkan perataan. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Mendapatkan atau mengatur teks alternatif badan untuk ikon file terlampir. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Mendapatkan atau mengatur judul teks alternatif untuk ikon file terlampir. |
| [getBytes()](#getBytes--) | Mendapatkan data biner untuk file tersemat. |
| [getExtension()](#getExtension--) | Mendapatkan ekstensi file tersemat. |
| [getFileName()](#getFileName--) | Mendapatkan nama file tersemat. |
| [getFilePath()](#getFilePath--) | Mendapatkan jalur ke file asli. |
| [getHeight()](#getHeight--) | Mendapatkan tinggi asli ikon file tersemat. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Mendapatkan offset horizontal. |
| [getIcon()](#getIcon--) | Mendapatkan data biner untuk ikon yang terkait dengan file tersemat. |
| [getIconExtension()](#getIconExtension--) | Mendapatkan ekstensi ikon. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan waktu terakhir dimodifikasi. |
| [getMaxHeight()](#getMaxHeight--) | Mendapatkan tinggi maksimum untuk menampilkan ikon file tersemat. |
| [getMaxWidth()](#getMaxWidth--) | Mendapatkan lebar maksimum untuk menampilkan ikon file tersemat. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Mendapatkan data tentang kesalahan yang terjadi saat mengakses file. |
| [getTags()](#getTags--) | Mendapatkan daftar tag dari file terlampir. |
| [getText()](#getText--) | Mendapatkan representasi teks dari file tersemat. |
| [getVerticalOffset()](#getVerticalOffset--) | Mendapatkan offset vertikal. |
| [getWidth()](#getWidth--) | Mendapatkan lebar asli ikon file tersemat. |
| [isPrintout()](#isPrintout--) | Mendapatkan nilai yang menunjukkan apakah tampilan file adalah cetakan. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Mendapatkan nilai yang menunjukkan apakah ukuran ikon secara eksplisit diperbarui oleh pengguna. |
| [setAlignment(int value)](#setAlignment-int-) | Mengatur perataan. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Mendapatkan atau mengatur teks alternatif badan untuk ikon file terlampir. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Mendapatkan atau mengatur judul teks alternatif untuk ikon file terlampir. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Mengatur offset horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mengatur waktu terakhir diubah. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Mengatur tinggi maksimum untuk menampilkan ikon file tersemat. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Mengatur lebar maksimum untuk menampilkan ikon file tersemat. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Mengatur nilai yang menunjukkan apakah tampilan file adalah cetakan. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Mengatur nilai yang menunjukkan apakah ukuran ikon secara eksplisit diperbarui oleh pengguna. |
| [setText(String value)](#setText-java.lang.String-) | Mengatur representasi teks dari file tersemat. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Mengatur offset vertikal. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Menginisialisasi sebuah instance baru dari kelas `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Sebuah string yang berisi jalur ke file yang akan digunakan untuk membuat `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Menginisialisasi sebuah instance baru dari kelas `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Sebuah string yang berisi jalur ke file yang akan digunakan untuk membuat `AttachedFile`. |
| icon | java.io.InputStream | Ikon untuk file terlampir. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Menginisialisasi sebuah instance baru dari kelas `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file terlampir. |
| attachedFileStream | java.io.InputStream | Aliran yang berisi byte file terlampir. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Menginisialisasi sebuah instance baru dari kelas `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file terlampir. |
| attachedFileStream | java.io.InputStream | Aliran yang berisi byte file terlampir. |
| icon | java.io.InputStream | Ikon untuk file terlampir. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Format ikon file terlampir. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Menginisialisasi sebuah instance baru dari kelas `AttachedFile`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Mendapatkan perataan.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Mendapatkan atau mengatur teks alternatif badan untuk ikon file terlampir.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Mendapatkan atau mengatur judul teks alternatif untuk ikon file terlampir.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Mendapatkan data biner untuk file tersemat.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Mendapatkan ekstensi file tersemat.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Mendapatkan nama file tersemat.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Mendapatkan jalur ke file asli.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Mendapatkan tinggi asli ikon file tersemat.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Mendapatkan offset horizontal.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Mendapatkan data biner untuk ikon yang terkait dengan file tersemat.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Mendapatkan ekstensi ikon.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Mendapatkan tinggi maksimum untuk menampilkan ikon file tersemat.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Mendapatkan lebar maksimum untuk menampilkan ikon file tersemat.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Mendapatkan data tentang kesalahan yang terjadi saat mengakses file.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Mendapatkan daftar tag dari file terlampir.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Mendapatkan representasi teks dari file tersemat. String tersebut TIDAK BOLEH mengandung karakter dengan nilai 10 (line feed) atau 13 (carriage return).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Mendapatkan offset vertikal.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Mendapatkan lebar asli ikon file tersemat.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Mendapatkan nilai yang menunjukkan apakah tampilan file adalah cetakan.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Mendapatkan nilai yang menunjukkan apakah ukuran ikon secara eksplisit diperbarui oleh pengguna.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Mengatur perataan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Nilai Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Mendapatkan atau mengatur teks alternatif badan untuk ikon file terlampir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Mendapatkan atau mengatur judul teks alternatif untuk ikon file terlampir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Mengatur offset horizontal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | Nilai Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mengatur waktu terakhir diubah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | Nilai Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Mengatur tinggi maksimum untuk menampilkan ikon file tersemat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | Nilai tinggi maksimum. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Mengatur lebar maksimum untuk menampilkan ikon file tersemat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | Nilai lebar maksimum. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Mengatur nilai yang menunjukkan apakah tampilan file adalah cetakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | Nilai baru. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Mengatur nilai yang menunjukkan apakah ukuran ikon secara eksplisit diperbarui oleh pengguna.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | Nilai baru. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Mengatur representasi teks dari file tersemat. String tersebut TIDAK BOLEH mengandung karakter dengan nilai 10 (line feed) atau 13 (carriage return).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Mengatur offset vertikal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | Nilai Offset. |

