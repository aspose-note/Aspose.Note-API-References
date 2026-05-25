---
title: "NotebookLoadOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Opsi yang digunakan untuk memuat notebook."
type: docs
weight: 58
url: /id/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Opsi yang digunakan untuk memuat notebook.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Menginisialisasi instance baru dari kelas `NotebookLoadOptions` kelas. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat secara eksplisit nanti. |
| [getInstantLoading()](#getInstantLoading--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat saat dokumen induk sedang dimuat. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat secara eksplisit nanti. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat saat dokumen induk sedang dimuat. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Menginisialisasi instance baru dari kelas `NotebookLoadOptions` kelas.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat secara eksplisit nanti.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan dimuat secara implisit. Nilai `true` menunjukkan bahwa pengguna harus memanggil `Notebook.loadChildDocument` atau untuk setiap node anak notebook setelah notebook itu sendiri dimuat. Jika nilai adalah `true`, opsi `NotebookLoadOptions.instantLoading` akan diabaikan. Jika notebook dimuat dari aliran, nilai selalu `true` meskipun secara eksplisit diatur oleh pengguna menjadi `false`.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat saat dokumen induk sedang dimuat.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan dimuat secara "malas", yaitu pemuatannya harus ditunda sampai ada akses langsung ke anak tertentu. Nilai `true` menunjukkan bahwa pemuatannya harus dilakukan segera.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat secara eksplisit nanti.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan dimuat secara implisit. Nilai `true` menunjukkan bahwa pengguna harus memanggil `Notebook.loadChildDocument` atau untuk setiap node anak notebook setelah notebook itu sendiri dimuat. Jika nilai adalah `true`, opsi `NotebookLoadOptions.instantLoading` akan diabaikan. Jika notebook dimuat dari aliran, nilai selalu `true` meskipun secara eksplisit diatur oleh pengguna menjadi `false`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah dokumen anak harus dimuat saat dokumen induk sedang dimuat.

--------------------

Nilai default adalah `false`, sehingga dokumen anak akan dimuat secara "malas", yaitu pemuatannya harus ditunda sampai ada akses langsung ke anak tertentu. Nilai `true` menunjukkan bahwa pemuatannya harus dilakukan segera.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

