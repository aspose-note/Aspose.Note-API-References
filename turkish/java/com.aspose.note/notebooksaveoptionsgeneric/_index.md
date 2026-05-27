---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note for Java API Referansı"
description: "Belirli bir format için defter kaydetme seçeneklerini temsil eden ve tüm belge alt düğümleri için ortak kaydetme seçenekleri sağlayan soyut bir temel sınıf."
type: docs
weight: 62
url: /tr/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Belirli bir format için defter kaydetme seçeneklerini temsil eden ve tüm belge alt düğümleri için ortak kaydetme seçenekleri sağlayan soyut bir temel sınıf.

`TDocumentSaveOptions`: Tüm not defterinin alt belgeleri için kaydetme seçenekleri.

TDocumentSaveOptions :
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Tüm not defterinin alt belgeleri için kaydetme seçeneklerini alır veya ayarlar. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Tüm notebook'un çocuk belgeleri için kaydetme seçeneklerini alır. |
| [getSaveFormat()](#getSaveFormat--) | Notebook'un kaydedildiği biçimi alır. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Tüm not defterinin alt belgeleri için kaydetme seçeneklerini alır veya ayarlar.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Tüm notebook'un çocuk belgeleri için kaydetme seçeneklerini alır.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Notebook'un kaydedildiği biçimi alır.

**Returns:**
int
