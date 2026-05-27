---
title: "NotebookSaveOptions"
second_title: "Aspose.Note for Java API Referansı"
description: "Belirli bir format için defter kaydetme seçeneklerini temsil eden soyut bir temel sınıf."
type: docs
weight: 61
url: /tr/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Belirli bir format için defter kaydetme seçeneklerini temsil eden soyut bir temel sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Çocuk belgelerin açıkça kaydedilmesi gerektiğini gösteren bir değeri alır veya ayarlar. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Tüm notebook'un çocuk belgeleri için kaydetme seçeneklerini alır. |
| [getFlatten()](#getFlatten--) | Notebook çocuk hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [getSaveFormat()](#getSaveFormat--) | Notebook'un kaydedildiği biçimi alır. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Çocuk belgelerin açıkça kaydedilmesi gerektiğini gösteren bir değeri alır veya ayarlar. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Notebook çocuk hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Çocuk belgelerin açıkça kaydedilmesi gerektiğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'dur, bu yüzden alt belgeler örtük olarak kaydedilir. `true` değeri, kullanıcının her defterin alt düğümünü açıkça kaydetmesi gerektiğini gösterir. Defter akışa kaydediliyorsa, değer her zaman `true` olur, kullanıcı tarafından açıkça `false` olarak ayarlanmış olsa bile.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Tüm notebook'un çocuk belgeleri için kaydetme seçeneklerini alır.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Notebook çocuk hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Notebook'un kaydedildiği biçimi alır.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Çocuk belgelerin açıkça kaydedilmesi gerektiğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'dur, bu yüzden alt belgeler örtük olarak kaydedilir. `true` değeri, kullanıcının her defterin alt düğümünü açıkça kaydetmesi gerektiğini gösterir. Defter akışa kaydediliyorsa, değer her zaman `true` olur, kullanıcı tarafından açıkça `false` olarak ayarlanmış olsa bile.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Notebook çocuk hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

