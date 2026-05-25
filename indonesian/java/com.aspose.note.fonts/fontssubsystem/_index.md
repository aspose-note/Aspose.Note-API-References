---
title: "FontsSubsystem"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar yang mengimplementasikan antarmuka com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /id/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Kelas dasar yang mengimplementasikan antarmuka com.aspose.note.IFontsSubsystem. Menyediakan fungsionalitas untuk font default dan substitusi font. Timpa fungsi anggota protected com.aspose.note.FontsSubsystem.fetchFontFamily dalam kelas turunan untuk menerapkan logika pengambilan objek Font.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Menambahkan font. |
| [addFont(String file)](#addFont-java.lang.String-) | Menambahkan font. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Menambahkan substitusi font. |
| [getDefaultFont()](#getDefaultFont--) | Mendapatkan font default. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Mendapatkan font. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Memuat semua font TrueType dari folder yang ditentukan ke koleksi internal. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Menambahkan font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Stream yang berisi font. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Menambahkan font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| file | java.lang.String | Jalur ke file yang berisi font. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Menambahkan substitusi font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| substituted | java.lang.String | Nama font yang disubstitusi. |
| substitution | java.lang.String | Nama font substitusi. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Mendapatkan font default.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Mendapatkan font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontName | java.lang.String | Nama font. |

**Returns:**
java.awt.Font - Font.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Memuat semua font TrueType dari folder yang ditentukan ke koleksi internal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| folder | java.lang.String | Folder yang berisi font. |

