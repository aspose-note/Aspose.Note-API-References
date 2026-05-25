---
title: "Lisensi"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Menyediakan metode untuk melisensikan komponen."
type: docs
weight: 44
url: /id/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Menyediakan metode untuk melisensikan komponen.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [License()](#License--) | Menginisialisasi instance baru dari kelas ini. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Mengatur ulang konteks lisensi untuk thread saat ini. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Memberi lisensi pada komponen. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Memberi lisensi pada komponen. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Memberi lisensi pada komponen. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Mengatur konteks lisensi untuk thread saat ini. |
### License() {#License--}
```
public License()
```


Menginisialisasi instance baru dari kelas ini.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Mengatur ulang konteks lisensi untuk thread saat ini.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Memberi lisensi pada komponen.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| licenseFile | java.io.File | File lisensi `System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Memberi lisensi pada komponen.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Aliran yang berisi lisensi. |

--------------------

`

Gunakan metode ini untuk memuat lisensi dari aliran.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Memberi lisensi pada komponen.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | licenseName | java.lang.String | Dapat berupa nama file lengkap atau pendek` atau nama sumber daya yang disematkan`. Gunakan string kosong untuk beralih ke mode evaluasi. |

--------------------

`

Mencoba menemukan lisensi di lokasi berikut:

` `

1. Jalur eksplisit.

` `

2. Folder yang berisi assembly komponen Aspose.

3. Folder yang berisi assembly pemanggilan klien.

4. Folder yang berisi assembly entri (startup).

5. Sumber daya yang disematkan dalam assembly pemanggilan klien.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Jalur eksplisit.

2. Sumber daya yang disematkan dalam assembly pemanggilan klien.

` `

2. Folder yang berisi file JAR komponen Aspose.

3. Folder yang berisi file JAR pemanggilan klien.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Mengatur konteks lisensi untuk thread saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran yang berisi lisensi. |

