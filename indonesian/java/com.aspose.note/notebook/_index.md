---
title: "Buku Catatan"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili notebook Aspose.Note."
type: docs
weight: 56
url: /id/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Mewakili notebook Aspose.Note.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Notebook()](#Notebook--) | Menginisialisasi instance baru dari kelas `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Menginisialisasi instance baru dari kelas `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Menginisialisasi instance baru dari kelas `Notebook`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Dapatkan semua node anak berdasarkan tipe node. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Menambahkan node ke akhir daftar. |
| [getColor()](#getColor--) | Mendapatkan atau mengatur warna. |
| [getCount()](#getCount--) | Mendapatkan jumlah elemen yang terdapat dalam `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Mendapatkan atau mengatur nama tampilan. |
| [getFileFormat()](#getFileFormat--) | Mendapatkan format file (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Mendapatkan id unik global objek. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Mendapatkan node anak notebook berdasarkan indeks yang diberikan. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah riwayat diaktifkan. |
| [iterator()](#iterator--) | Mengembalikan enumerator yang mengiterasi node anak dari `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Menambahkan node dokumen anak. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Menambahkan node dokumen anak. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Menambahkan node dokumen anak. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Menambahkan node dokumen anak. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Menambahkan node notebook anak. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Menambahkan node notebook anak. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Menghapus node anak. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Menyimpan dokumen OneNote ke aliran. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan. |
| [save(String fileName)](#save-java.lang.String-) | Menyimpan dokumen OneNote ke file. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Menyimpan dokumen OneNote ke file dalam format yang ditentukan. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Mendapatkan atau mengatur warna. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Mendapatkan atau mengatur nama tampilan. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah riwayat diaktifkan. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Menginisialisasi instance baru dari kelas `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Menginisialisasi instance baru dari kelas `Notebook`. Membuka notebook OneNote yang ada dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas `Notebook`. Membuka notebook OneNote yang ada dari sebuah file. Memungkinkan untuk menentukan opsi tambahan seperti strategi pemuatan anak (\"lazy\"/instant).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Opsi pemuatan. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Dapatkan semua node anak berdasarkan tipe node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Daftar node anak.

`T1`: Tipe elemen dalam daftar yang dikembalikan.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Menambahkan node ke akhir daftar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Node yang akan ditambahkan. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Mendapatkan atau mengatur warna.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Mendapatkan jumlah elemen yang terdapat dalam `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Mendapatkan atau mengatur nama tampilan.

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

Nilai: GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Mendapatkan node anak notebook berdasarkan indeks yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Indeks ke node anak. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah riwayat diaktifkan.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Mengembalikan enumerator yang mengiterasi node anak dari `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Sebuah `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Menambahkan node dokumen anak. Membuka dokumen OneNote yang ada dari sebuah stream.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Menambahkan node dokumen anak. Membuka dokumen OneNote yang ada dari sebuah stream. Memungkinkan untuk menentukan opsi pemuatan tambahan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi pemuatan. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Menambahkan node dokumen anak. Membuka dokumen OneNote yang ada dari sebuah file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Menambahkan node dokumen anak. Membuka dokumen OneNote yang ada dari sebuah file. Memungkinkan untuk menentukan opsi pemuatan tambahan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Opsi pemuatan. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Menambahkan node notebook anak. Membuka notebook OneNote yang ada dari sebuah file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Menambahkan node notebook anak. Membuka notebook OneNote yang ada dari sebuah file. Memungkinkan untuk menentukan opsi pemuatan tambahan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | Jalur file. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Opsi pemuatan. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Menghapus node anak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Node yang akan dihapus. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Menyimpan dokumen OneNote ke aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | Aliran. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Menyimpan dokumen OneNote ke aliran menggunakan opsi penyimpanan yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | Aliran. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Menentukan opsi bagaimana dokumen disimpan. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Menyimpan dokumen OneNote ke aliran dalam format yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | Aliran. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Menyimpan dokumen OneNote ke file menggunakan opsi penyimpanan yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama lengkap untuk file. Jika file dengan nama lengkap yang ditentukan sudah ada, file yang ada akan ditimpa. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Menentukan opsi bagaimana dokumen disimpan dalam file. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Mendapatkan atau mengatur warna.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Mendapatkan atau mengatur nama tampilan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah riwayat diaktifkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

