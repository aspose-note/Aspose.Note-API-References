---
title: "NotebookSaveOptionsGeneric"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu dan menyediakan opsi penyimpanan umum untuk semua node anak dokumen."
type: docs
weight: 62
url: /id/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Kelas dasar abstrak yang mewakili opsi penyimpanan notebook untuk format tertentu dan menyediakan opsi penyimpanan umum untuk semua node anak dokumen.

`TDocumentSaveOptions`: Opsi penyimpanan untuk semua dokumen anak notebook.

TDocumentSaveOptions :
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Mendapatkan atau mengatur opsi penyimpanan untuk semua dokumen anak notebook. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Mendapatkan opsi penyimpanan untuk semua dokumen anak notebook. |
| [getSaveFormat()](#getSaveFormat--) | Mendapatkan format di mana notebook disimpan. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Mendapatkan atau mengatur opsi penyimpanan untuk semua dokumen anak notebook.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Mendapatkan opsi penyimpanan untuk semua dokumen anak notebook.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Mendapatkan format di mana notebook disimpan.

**Returns:**
int
