---
title: "Gambar"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili sebuah Gambar."
type: docs
weight: 33
url: /id/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Mewakili sebuah Gambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Menginisialisasi instance baru dari kelas `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Menginisialisasi instance baru dari kelas `Image`. |
| [Image()](#Image--) | Menginisialisasi instance baru dari kelas `Image`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [getAlignment()](#getAlignment--) | Mendapatkan perataan. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Mendapatkan teks alternatif badan untuk gambar. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Mendapatkan judul teks alternatif untuk gambar. |
| [getBytes()](#getBytes--) | Mendapatkan penyimpanan data gambar. |
| [getFileName()](#getFileName--) | Mendapatkan nama file. |
| [getFilePath()](#getFilePath--) | Mendapatkan jalur ke file gambar. |
| [getFormat()](#getFormat--) | Mendapatkan format gambar. |
| [getHeight()](#getHeight--) | Mendapatkan tinggi. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Mendapatkan offset horizontal. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Mendapatkan hyperlink yang terkait dengan gambar. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan waktu terakhir dimodifikasi. |
| [getOriginalHeight()](#getOriginalHeight--) | Mendapatkan tinggi asli. |
| [getOriginalWidth()](#getOriginalWidth--) | Mendapatkan lebar asli. |
| [getTags()](#getTags--) | Mendapatkan daftar semua tag gambar. |
| [getVerticalOffset()](#getVerticalOffset--) | Mendapatkan offset vertikal. |
| [getWidth()](#getWidth--) | Mendapatkan lebar. |
| [isBackground()](#isBackground--) | Mendapatkan apakah gambar merupakan gambar latar belakang. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Mengganti data gambar saat ini dengan data dari objek `Image` yang disediakan. |
| [setAlignment(int value)](#setAlignment-int-) | Mengatur perataan. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Mengatur teks alternatif badan untuk gambar. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Mengatur judul teks alternatif untuk gambar. |
| [setBackground(boolean value)](#setBackground-boolean-) | Mendapatkan apakah gambar merupakan gambar latar belakang. |
| [setHeight(float value)](#setHeight-float-) | Mengatur tinggi. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Mengatur offset horizontal. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Mengatur hyperlink yang terkait dengan gambar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mengatur waktu terakhir dimodifikasi. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Mengatur offset vertikal. |
| [setWidth(float value)](#setWidth-float-) | Mengatur lebar. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Menginisialisasi instance baru dari kelas `Image`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | String yang berisi jalur ke file dari mana membuat `Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Menginisialisasi instance baru dari kelas `Image`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama gambar. |
| imageStream | java.io.InputStream | Stream yang berisi gambar. |

### Image() {#Image--}
```
public Image()
```


Menginisialisasi instance baru dari kelas `Image`.

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


Mendapatkan teks alternatif badan untuk gambar.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Mendapatkan judul teks alternatif untuk gambar.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Mendapatkan penyimpanan data gambar.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Mendapatkan nama file.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Mendapatkan jalur ke file gambar.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Mendapatkan format gambar.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Mendapatkan tinggi. Ini adalah tinggi sebenarnya dari gambar dalam dokumen MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Mendapatkan offset horizontal.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Mendapatkan hyperlink yang terkait dengan gambar.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Mendapatkan tinggi asli. Ini adalah lebar asli gambar, sebelum diubah ukurannya.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Mendapatkan lebar asli. Ini adalah lebar asli gambar, sebelum diubah ukurannya.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Mendapatkan daftar semua tag gambar.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Mendapatkan offset vertikal.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Mendapatkan lebar. Ini adalah lebar sebenarnya dari gambar dalam dokumen MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Mendapatkan apakah gambar merupakan gambar latar belakang.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Mengganti data gambar saat ini dengan data dari objek `Image` yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Mengatur perataan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Mengatur teks alternatif badan untuk gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Mengatur judul teks alternatif untuk gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Mendapatkan apakah gambar merupakan gambar latar belakang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Mengatur tinggi. Ini adalah tinggi sebenarnya dari gambar dalam dokumen MS OneNote.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Mengatur offset horizontal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Mengatur hyperlink yang terkait dengan gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mengatur waktu terakhir dimodifikasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Mengatur offset vertikal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Mengatur lebar. Ini adalah lebar sebenarnya dari gambar dalam dokumen MS OneNote.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float |  |

