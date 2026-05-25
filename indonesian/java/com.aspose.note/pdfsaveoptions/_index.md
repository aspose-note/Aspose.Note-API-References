---
title: "PdfSaveOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen ke PDF."
type: docs
weight: 77
url: /id/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Memungkinkan untuk menentukan opsi tambahan saat merender halaman dokumen ke PDF.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Menginisialisasi instance baru dari kelas `PdfSaveOptions`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Mendapatkan tipe kompresi yang diterapkan pada gambar dalam file PDF. |
| [getJpegQuality()](#getJpegQuality--) | Mendapatkan nilai yang menentukan kualitas gambar JPEG dalam dokumen PDF. |
| [getPageSettings()](#getPageSettings--) | Mendapatkan atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Mendapatkan atau mengatur algoritma yang digunakan untuk pemisahan halaman. |
| [setImageCompression(int value)](#setImageCompression-int-) | Mengatur tipe kompresi yang diterapkan pada gambar dalam file PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Mengatur nilai yang menentukan kualitas gambar JPEG dalam dokumen PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Mendapatkan atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Mendapatkan atau mengatur algoritma yang digunakan untuk pemisahan halaman. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Menginisialisasi instance baru dari kelas `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Mendapatkan tipe kompresi yang diterapkan pada gambar dalam file PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Mendapatkan nilai yang menentukan kualitas gambar JPEG dalam dokumen PDF. Nilai dapat bervariasi dari 0 hingga 100 dimana 0 berarti kualitas terburuk tetapi kompresi maksimum dan 100 berarti kualitas terbaik tetapi kompresi minimum.

--------------------

Nilai default adalah 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Mendapatkan atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. Secara default tergantung pada CurrentUICulture, \*US cultures memiliki pengaturan letter, yang lain memiliki pengaturan A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Mendapatkan atau mengatur algoritma yang digunakan untuk pemisahan halaman.

Nilai: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Mengatur tipe kompresi yang diterapkan pada gambar dalam file PDF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Mengatur nilai yang menentukan kualitas gambar JPEG dalam dokumen PDF. Nilai dapat bervariasi dari 0 hingga 100 dimana 0 berarti kualitas terburuk tetapi kompresi maksimum dan 100 berarti kualitas terbaik tetapi kompresi minimum.

--------------------

Nilai default adalah 90.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Mendapatkan atau mengatur pengaturan halaman untuk setiap halaman dalam dokumen. Secara default tergantung pada CurrentUICulture, \*US cultures memiliki pengaturan letter, yang lain memiliki pengaturan A4.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Mendapatkan atau mengatur algoritma yang digunakan untuk pemisahan halaman.

Nilai: `PageSplittingAlgorithm`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

