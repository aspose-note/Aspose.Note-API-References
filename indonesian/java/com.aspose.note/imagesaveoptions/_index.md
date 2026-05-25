---
title: "ImageSaveOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Memungkinkan menentukan opsi tambahan saat merender halaman dokumen menjadi gambar."
type: docs
weight: 35
url: /id/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Memungkinkan menentukan opsi tambahan saat merender halaman dokumen menjadi gambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Menginisialisasi instance baru dari kelas `ImageSaveOptions`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Mendapatkan atau mengatur opsi untuk binarisasi gambar. |
| [getColorMode()](#getColorMode--) | Mendapatkan atau mengatur `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) untuk gambar output. |
| [getQuality()](#getQuality--) | Mendapatkan nilai yang menentukan kualitas gambar yang disimpan. |
| [getResolution()](#getResolution--) | Mendapatkan resolusi untuk gambar yang dihasilkan, dalam titik per inci. |
| [getTiffCompression()](#getTiffCompression--) | Mendapatkan atau mengatur jenis kompresi yang digunakan saat menyimpan gambar yang dihasilkan ke format TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Mendapatkan atau mengatur opsi untuk binarisasi gambar. |
| [setColorMode(int value)](#setColorMode-int-) | Mendapatkan atau mengatur `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) untuk gambar output. |
| [setQuality(int value)](#setQuality-int-) | Mengatur nilai yang menentukan kualitas gambar yang disimpan. |
| [setResolution(float value)](#setResolution-float-) | Mengatur resolusi untuk gambar yang dihasilkan, dalam dot per inci. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Mendapatkan atau mengatur jenis kompresi yang digunakan saat menyimpan gambar yang dihasilkan ke format TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Menginisialisasi instance baru dari kelas `ImageSaveOptions`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| format | int | Format di mana dokumen disimpan. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Mendapatkan atau mengatur opsi untuk binarisasi gambar.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Mendapatkan atau mengatur `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) untuk gambar output.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Mendapatkan nilai yang menentukan kualitas gambar yang disimpan. Nilai ini diteruskan ke codec sebagai parameter System.Drawing.Imaging.Encoder.Quality.

--------------------

Rentang nilai yang berguna untuk kategori kualitas adalah dari 0 hingga 100. Semakin rendah angka yang ditentukan, semakin tinggi kompresi dan oleh karena itu kualitas gambar semakin rendah. Nol akan memberikan gambar dengan kualitas terendah dan 100 yang tertinggi. Nilai default adalah 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Mendapatkan resolusi untuk gambar yang dihasilkan, dalam titik per inci.

--------------------

Nilai default adalah 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Mendapatkan atau mengatur jenis kompresi yang digunakan saat menyimpan gambar yang dihasilkan ke format TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Mendapatkan atau mengatur opsi untuk binarisasi gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Mendapatkan atau mengatur `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) untuk gambar output.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Mengatur nilai yang menentukan kualitas gambar yang disimpan. Nilai ini diteruskan ke codec sebagai parameter System.Drawing.Imaging.Encoder.Quality.

--------------------

Rentang nilai yang berguna untuk kategori kualitas adalah dari 0 hingga 100. Semakin rendah angka yang ditentukan, semakin tinggi kompresi dan oleh karena itu kualitas gambar semakin rendah. Nol akan memberikan gambar dengan kualitas terendah dan 100 yang tertinggi. Nilai default adalah 90.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Mengatur resolusi untuk gambar yang dihasilkan, dalam dot per inci.

--------------------

Nilai default adalah 90.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Mendapatkan atau mengatur jenis kompresi yang digunakan saat menyimpan gambar yang dihasilkan ke format TIFF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

