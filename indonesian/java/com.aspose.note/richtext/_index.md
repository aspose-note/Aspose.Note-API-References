---
title: "RichText"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili teks kaya."
type: docs
weight: 82
url: /id/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Mewakili teks kaya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [RichText()](#RichText--) | Menginisialisasi instance baru dari kelas [RichText](../../com.aspose.note/richtext). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [append(String value)](#append-java.lang.String-) | Menambahkan string ke rentang teks terakhir. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Menambahkan string ke akhir. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Menambahkan string ke depan rentang teks pertama. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Menambahkan string ke depan. |
| [clear()](#clear--) | Menghapus konten instance ini. |
| [getAlignment()](#getAlignment--) | Mendapatkan perataan. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan waktu terakhir dimodifikasi. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Mendapatkan jarak baris. |
| [getParagraphStyle()](#getParagraphStyle--) | Mendapatkan gaya paragraf. |
| [getSpaceAfter()](#getSpaceAfter--) | Mendapatkan jumlah minimum ruang setelah. |
| [getSpaceBefore()](#getSpaceBefore--) | Mendapatkan jumlah minimum ruang sebelum. |
| [getStyles()](#getStyles--) | Mendapatkan gaya. |
| [getTags()](#getTags--) | Mendapatkan daftar semua tag dari sebuah paragraf. |
| [getText()](#getText--) | Mendapatkan teks. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Mengembalikan indeks berbasis nol dari kemunculan pertama karakter yang ditentukan dalam instance ini. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Menyisipkan string yang ditentukan pada posisi indeks yang ditentukan dalam instance ini. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Menyisipkan string yang ditentukan dengan gaya yang ditentukan pada posisi indeks yang ditentukan dalam instance ini. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Menghapus semua karakter dalam instance saat ini, mulai dari posisi yang ditentukan dan berlanjut hingga posisi terakhir. |
| [remove(int startIndex, int count)](#remove-int-int-) | Menghapus sejumlah karakter yang ditentukan dalam instance saat ini mulai dari posisi yang ditentukan. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Mengganti semua kemunculan karakter Unicode yang ditentukan dalam instance ini dengan karakter Unicode lain yang ditentukan. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Mengganti semua kemunculan string yang ditentukan dalam instance saat ini dengan string lain yang ditentukan. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Mengganti semua kemunculan string yang ditentukan dalam instance saat ini dengan string lain yang ditentukan dalam gaya yang ditentukan. |
| [setAlignment(int value)](#setAlignment-int-) | Mengatur perataan. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mengatur waktu terakhir diubah. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Mengatur jarak baris. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Mengatur gaya paragraf. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Mengatur jumlah minimum ruang setelah. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Mengatur jumlah minimum ruang sebelum. |
| [setText(String value)](#setText-java.lang.String-) | Mengatur teks. |
| [trim()](#trim--) | Menghapus semua karakter spasi putih di awal dan akhir. |
| [trim(char trimChar)](#trim-char-) | Menghapus semua kemunculan karakter di awal dan akhir. |
| [trim(char[] trimChars)](#trim-char...-) | Menghapus semua kemunculan set karakter yang ditentukan dalam array di awal dan akhir. |
| [trimEnd()](#trimEnd--) | Menghapus semua karakter spasi putih di akhir. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Menghapus semua kemunculan karakter di akhir. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Menghapus semua kemunculan set karakter yang ditentukan dalam array di akhir. |
| [trimStart()](#trimStart--) | Menghapus semua karakter spasi putih di awal. |
| [trimStart(char trimChar)](#trimStart-char-) | Menghapus semua kemunculan karakter yang ditentukan di awal. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Menghapus semua kemunculan set karakter yang ditentukan dalam array di awal. |
### RichText() {#RichText--}
```
public RichText()
```


Menginisialisasi instance baru dari kelas [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Menambahkan string ke rentang teks terakhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai yang ditambahkan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Menambahkan string ke akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai yang ditambahkan. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Gaya string yang ditambahkan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Menambahkan string ke depan rentang teks pertama.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai yang ditambahkan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Menambahkan string ke depan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai yang ditambahkan. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Gaya string yang ditambahkan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Menghapus konten instance ini.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Mendapatkan perataan.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Mendapatkan jarak baris.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Mendapatkan gaya paragraf. Pengaturan ini digunakan jika tidak ada objek TextStyle yang cocok dalam koleksi [getStyles](../../com.aspose.note/richtext\\#getStyles) atau objek ini tidak menentukan pengaturan yang diperlukan.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Mendapatkan jumlah minimum ruang setelah.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Mendapatkan jumlah minimum ruang sebelum.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Mendapatkan gaya.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Mendapatkan daftar semua tag dari sebuah paragraf.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Mendapatkan teks. String INI TIDAK BOLEH mengandung karakter dengan nilai 10 (line feed).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char | Nilai. |

**Returns:**
int - `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama karakter Unicode yang ditentukan dalam string ini. Pencarian dimulai pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char | Nilai. |
| startIndex | int | Posisi pencarian awal |

**Returns:**
int - `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama karakter yang ditentukan dalam instance ini. Pencarian dimulai pada posisi karakter yang ditentukan dan memeriksa sejumlah posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char | Nilai. |
| startIndex | int | Posisi pencarian awal |
| count | int | Jumlahnya. |

**Returns:**
int - `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |

**Returns:**
int - `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini. Pencarian dimulai pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |
| startIndex | int | Posisi pencarian awal |

**Returns:**
int - `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance ini. Pencarian dimulai pada posisi karakter yang ditentukan dan memeriksa sejumlah posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |
| startIndex | int | Posisi pencarian awal |
| count | int | Jumlahnya. |

**Returns:**
int - `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |
| startIndex | int | Posisi pencarian awal |
| count | int | Jumlahnya. |
| comparisonType | short | Tipe pencarian yang digunakan untuk string yang ditentukan |

**Returns:**
int - `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. Sebuah parameter menentukan tipe pencarian yang digunakan untuk string yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |
| comparisonType | short | Tipe pencarian yang digunakan untuk string yang ditentukan |

**Returns:**
int - `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Mengembalikan indeks berbasis nol dari kemunculan pertama string yang ditentukan dalam instance saat ini. Parameter menentukan posisi awal pencarian dalam string saat ini dan tipe pencarian yang digunakan untuk string yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai. |
| startIndex | int | Posisi pencarian awal |
| comparisonType | short | Tipe pencarian yang digunakan untuk string yang ditentukan |

**Returns:**
int - `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Menyisipkan string yang ditentukan pada posisi indeks yang ditentukan dalam instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Indeks awal. |
| nilai | java.lang.String | Nilai. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Menyisipkan string yang ditentukan dengan gaya yang ditentukan pada posisi indeks yang ditentukan dalam instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Indeks awal. |
| nilai | java.lang.String | Nilai. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Gaya. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Menghapus semua karakter dalam instance saat ini, mulai dari posisi yang ditentukan dan berlanjut hingga posisi terakhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Indeks awal. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Menghapus sejumlah karakter yang ditentukan dalam instance saat ini mulai dari posisi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Indeks awal. |
| count | int | Jumlahnya. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Mengganti semua kemunculan karakter Unicode yang ditentukan dalam instance ini dengan karakter Unicode lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldChar | char | Karakter lama. |
| newChar | char | Karakter baru. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Mengganti semua kemunculan string yang ditentukan dalam instance saat ini dengan string lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldValue | java.lang.String | Nilai lama. |
| newValue | java.lang.String | Nilai baru. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Mengganti semua kemunculan string yang ditentukan dalam instance saat ini dengan string lain yang ditentukan dalam gaya yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldValue | java.lang.String | Nilai lama. |
| newValue | java.lang.String | Nilai baru. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Gaya nilai baru. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Mengatur perataan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mengatur waktu terakhir diubah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Mengatur jarak baris.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Mengatur gaya paragraf. Pengaturan ini digunakan jika tidak ada objek TextStyle yang cocok dalam koleksi [getStyles](../../com.aspose.note/richtext\\#getStyles) atau objek ini tidak menentukan pengaturan yang diperlukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Mengatur jumlah minimum ruang setelah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Mengatur jumlah minimum ruang sebelum.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Mengatur teks. String INI TIDAK BOLEH mengandung karakter dengan nilai 10 (line feed).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Menghapus semua karakter spasi putih di awal dan akhir.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Menghapus semua kemunculan karakter di awal dan akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChar | char | Karakter pemotongan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Menghapus semua kemunculan set karakter yang ditentukan dalam array di awal dan akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChars | char[] | Karakter pemangkasan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Menghapus semua karakter spasi putih di akhir.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Menghapus semua kemunculan karakter di akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChar | char | Karakter pemotongan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Menghapus semua kemunculan set karakter yang ditentukan dalam array di akhir.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChars | char[] | Karakter pemangkasan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Menghapus semua karakter spasi putih di awal.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Menghapus semua kemunculan karakter yang ditentukan di awal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChar | char | Karakter pemotongan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Menghapus semua kemunculan set karakter yang ditentukan dalam array di awal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| trimChars | char[] | Karakter pemangkasan. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
