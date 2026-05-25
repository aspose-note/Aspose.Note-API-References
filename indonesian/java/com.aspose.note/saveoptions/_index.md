---
title: "SaveOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar abstrak yang mewakili opsi penyimpanan dokumen untuk format tertentu."
type: docs
weight: 85
url: /id/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Kelas dasar abstrak yang mewakili opsi penyimpanan dokumen untuk format tertentu.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Mendapatkan atau mengatur pengaturan font yang akan digunakan saat menyimpan |
| [getPageCount()](#getPageCount--) | Mendapatkan atau mengatur jumlah halaman yang akan disimpan. |
| [getPageIndex()](#getPageIndex--) | Mendapatkan atau mengatur indeks halaman pertama yang akan disimpan. |
| [getSaveFormat()](#getSaveFormat--) | Mendapatkan atau mengatur format di mana dokumen disimpan. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Mendapatkan atau mengatur pengaturan font yang akan digunakan saat menyimpan |
| [setPageCount(int value)](#setPageCount-int-) | Mendapatkan atau mengatur jumlah halaman yang akan disimpan. |
| [setPageIndex(int value)](#setPageIndex-int-) | Mendapatkan atau mengatur indeks halaman pertama yang akan disimpan. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Mendapatkan atau mengatur pengaturan font yang akan digunakan saat menyimpan

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Mendapatkan atau mengatur jumlah halaman yang akan disimpan. Secara default adalah \{@link int\#Int32Extensions.MaxValue\} yang berarti semua halaman dokumen akan dirender.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Mendapatkan atau mengatur indeks halaman pertama yang akan disimpan. Secara default adalah 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Mendapatkan atau mengatur format di mana dokumen disimpan.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Mendapatkan atau mengatur pengaturan font yang akan digunakan saat menyimpan

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Mendapatkan atau mengatur jumlah halaman yang akan disimpan. Secara default adalah \{@link int\#Int32Extensions.MaxValue\} yang berarti semua halaman dokumen akan dirender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Mendapatkan atau mengatur indeks halaman pertama yang akan disimpan. Secara default adalah 0.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

