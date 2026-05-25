---
title: "DocumentFontsSubsystem"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Implementasi sederhana dari Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /id/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Implementasi sederhana dari Aspose.Note.Fonts.FontsSubsystem. Mengambil objek FontFamily dari OS.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDefault()](#getDefault--) | Mendapatkan atau mengatur instance default statis. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Mendapatkan atau mengatur instance default statis. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Buat instance DocumentFontsSubsystem baru menggunakan font dari file yang ditentukan sebagai default. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Aliran yang berisi Font default. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Aliran yang berisi Font default. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Jalur ke file yang berisi Font default. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Jalur ke file yang berisi Font default. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Menginisialisasi instance baru dari kelas [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Mendapatkan atau mengatur instance default statis.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Mendapatkan atau mengatur instance default statis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontName | java.lang.String | Nama font default. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontName | java.lang.String | Nama font default. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Buat instance DocumentFontsSubsystem baru menggunakan nama font default yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | File yang berisi nama font default. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Buat instance DocumentFontsSubsystem baru menggunakan font dari file yang ditentukan sebagai default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | File yang berisi nama font default. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Aliran yang berisi nama font default. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Buat instance DocumentFontsSubsystem baru menggunakan font dari aliran yang ditentukan sebagai default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Aliran yang berisi nama font default. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Substitusi font. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
