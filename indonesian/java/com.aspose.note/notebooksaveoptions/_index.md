---
title: "NotebookSaveOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu."
type: docs
weight: 61
url: /id/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus disimpan secara eksplisit. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Mendapatkan opsi penyimpanan untuk semua dokumen anak notebook. |
| [getFlatten()](#getFlatten--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah hierarki anak notebook disimpan secara rata. |
| [getSaveFormat()](#getSaveFormat--) | Mendapatkan format di mana notebook disimpan. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus disimpan secara eksplisit. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah hierarki anak notebook disimpan secara rata. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus disimpan secara eksplisit.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan disimpan secara implisit. Nilai `true` menunjukkan bahwa pengguna harus menyimpan setiap node anak notebook secara eksplisit. Jika notebook disimpan ke stream, nilai selalu `true` meskipun sebelumnya secara eksplisit diatur oleh pengguna menjadi `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Mendapatkan opsi penyimpanan untuk semua dokumen anak notebook.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah hierarki anak notebook disimpan secara rata.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Mendapatkan format di mana notebook disimpan.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus disimpan secara eksplisit.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan disimpan secara implisit. Nilai `true` menunjukkan bahwa pengguna harus menyimpan setiap node anak notebook secara eksplisit. Jika notebook disimpan ke stream, nilai selalu `true` meskipun sebelumnya secara eksplisit diatur oleh pengguna menjadi `false`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah hierarki anak notebook disimpan secara rata.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

