---
title: "Document"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili dokumen Aspose.Note."
type: docs
weight: 20
url: /id/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Mewakili dokumen Aspose.Note.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Document()](#Document--) | Menginisialisasi sebuah instance baru dari kelas `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Menginisialisasi sebuah instance baru dari kelas `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Menginisialisasi sebuah instance baru dari kelas `Document`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Menerima pengunjung node. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Mendeteksi semua perubahan yang dibuat pada tata letak dokumen sejak pemanggilan `DetectLayoutChanges` sebelumnya. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Mendapatkan nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis. |
| [getColor()](#getColor--) | Mendapatkan warna. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan waktu pembuatan. |
| [getDisplayName()](#getDisplayName--) | Mendapatkan nama tampilan. |
| [getFileFormat()](#getFileFormat--) | Mendapatkan format file (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Mendapatkan id unik global objek. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Mendapatkan `PageHistory` yang berisi riwayat lengkap untuk setiap halaman yang ditampilkan dalam dokumen (yang paling awal pada indeks 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Memeriksa apakah dokumen dari aliran dienkripsi. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Memeriksa apakah dokumen dari aliran dienkripsi. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Memeriksa apakah dokumen dari aliran dienkripsi. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Memeriksa apakah dokumen dari file dienkripsi. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Memeriksa apakah dokumen dari file dienkripsi. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Memeriksa apakah dokumen dari file dienkripsi. |
| [print()](#print--) | Mencetak dokumen menggunakan printer default. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Mencetak dokumen menggunakan printer default. |
| [print(String printerName)](#print-java.lang.String-) | Mencetak dokumen menggunakan printer default. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Mencetak dokumen menggunakan printer default. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Menyimpan dokumen OneNote ke aliran. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan. |
| [save(String fileName)](#save-java.lang.String-) | Menyimpan dokumen OneNote ke file. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Menyimpan dokumen OneNote ke file dalam format yang ditentukan. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Mengatur nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Mengatur warna. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Mengatur waktu pembuatan. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Mengatur nama tampilan. |
### Document() {#Document--}
```
public Document()
```


Menginisialisasi instance baru dari kelas `Document`. Membuat dokumen OneNote kosong.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Menginisialisasi instance baru dari kelas `Document`. Membuka dokumen OneNote yang ada dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas `Document`. Membuka dokumen OneNote yang ada dari file. Memungkinkan untuk menentukan opsi tambahan seperti kata sandi enkripsi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi yang digunakan untuk memuat dokumen. Dapat bernilai null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Menginisialisasi instance baru dari kelas `Document`. Membuka dokumen OneNote yang ada dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inStream | java.io.InputStream | Aliran. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas `Document`. Membuka dokumen OneNote yang ada dari aliran. Memungkinkan untuk menentukan opsi tambahan seperti kata sandi enkripsi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inStream | java.io.InputStream | Aliran. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi yang digunakan untuk memuat dokumen. Dapat bernilai null. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Menerima pengunjung node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objek dari kelas yang diturunkan dari `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Mendeteksi semua perubahan yang dibuat pada tata letak dokumen sejak pemanggilan `DetectLayoutChanges` sebelumnya. Jika `AutomaticLayoutChangesDetectionEnabled` diatur ke true, akan digunakan secara otomatis pada awal ekspor dokumen.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Mendapatkan nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis. Nilai default adalah `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Mendapatkan warna.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Mendapatkan waktu pembuatan.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Mendapatkan nama tampilan.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Mendapatkan format file (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Mendapatkan id unik global objek.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Mendapatkan `PageHistory` yang berisi riwayat lengkap untuk setiap halaman yang ditampilkan dalam dokumen (yang paling awal pada indeks 0). Revisi halaman saat ini dapat diakses sebagai `PageHistory.current` dan disimpan terpisah dari koleksi versi historis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Revisi saat ini dari sebuah halaman. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi pemuatan. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran. |
| password | java.lang.String | Kata sandi untuk mendekripsi dokumen. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi pemuatan. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| password | java.lang.String | Kata sandi untuk mendekripsi dokumen. |
| document | [Document\[\]](../../com.aspose.note/document) | Dokumen yang dimuat. |

**Returns:**
boolean - Mengembalikan true jika dokumen dienkripsi, jika tidak false.
### print() {#print--}
```
public void print()
```


Mencetak dokumen menggunakan printer default.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Mencetak dokumen menggunakan printer default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Opsi yang digunakan untuk mencetak dokumen. Bisa bernilai null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Mencetak dokumen menggunakan printer default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Mencetak dokumen menggunakan printer default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Menyimpan dokumen OneNote ke aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | System.iO.stream tempat dokumen akan disimpan. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | System.iO.stream tempat dokumen akan disimpan. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Menentukan opsi bagaimana dokumen disimpan dalam stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | System.iO.stream tempat dokumen akan disimpan. |
| format | int | Format di mana dokumen akan disimpan. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Menyimpan dokumen OneNote ke file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama lengkap untuk file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama lengkap untuk file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Menentukan opsi bagaimana dokumen disimpan dalam file. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Menyimpan dokumen OneNote ke file dalam format yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama lengkap untuk file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |
| format | int | Format di mana dokumen akan disimpan. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Mengatur nilai yang menunjukkan apakah Aspose.Note melakukan deteksi perubahan tata letak secara otomatis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | Nilai baru. Bisa bernilai null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Mengatur warna.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | Nilai Color. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Mengatur waktu pembuatan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | Nilai DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Mengatur nama tampilan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | Nilai DateTime. |

