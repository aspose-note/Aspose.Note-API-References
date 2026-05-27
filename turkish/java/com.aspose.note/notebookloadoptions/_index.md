---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir defteri yüklemek için kullanılan seçenekler."
type: docs
weight: 58
url: /tr/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Bir defteri yüklemek için kullanılan seçenekler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | `NotebookLoadOptions` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | Çocuk belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [getInstantLoading()](#getInstantLoading--) | Çocuk belgelerin üst belge yüklenirken yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Çocuk belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Çocuk belgelerin üst belge yüklenirken yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


`NotebookLoadOptions` sınıfının yeni bir örneğini başlatır.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Çocuk belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'tur, bu yüzden alt belgeler örtük olarak yüklenecektir. `true` değeri, kullanıcının `Notebook.loadChildDocument` metodunu çağırması veya defter yüklendikten sonra her defter alt düğümü için çağırması gerektiğini gösterir. Değer `true` ise, `NotebookLoadOptions.instantLoading` seçeneği yok sayılacaktır. Defter bir akıştan yükleniyorsa, değer kullanıcı tarafından açıkça `false` olarak ayarlanmış olsa bile her zaman `true` olur.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Çocuk belgelerin üst belge yüklenirken yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'tur, bu yüzden alt belgeler "tembel" bir şekilde yüklenecektir, yani yüklemeleri belirli bir alt öğeye doğrudan erişilene kadar ertelenmelidir. `true` değeri, yüklemelerinin hemen yapılması gerektiğini gösterir.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Çocuk belgelerin daha sonra açıkça yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'tur, bu yüzden alt belgeler örtük olarak yüklenecektir. `true` değeri, kullanıcının `Notebook.loadChildDocument` metodunu çağırması veya defter yüklendikten sonra her defter alt düğümü için çağırması gerektiğini gösterir. Değer `true` ise, `NotebookLoadOptions.instantLoading` seçeneği yok sayılacaktır. Defter bir akıştan yükleniyorsa, değer kullanıcı tarafından açıkça `false` olarak ayarlanmış olsa bile her zaman `true` olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Çocuk belgelerin üst belge yüklenirken yüklenip yüklenmeyeceğini gösteren bir değeri alır veya ayarlar.

--------------------

Varsayılan değer `false`'tur, bu yüzden alt belgeler "tembel" bir şekilde yüklenecektir, yani yüklemeleri belirli bir alt öğeye doğrudan erişilene kadar ertelenmelidir. `true` değeri, yüklemelerinin hemen yapılması gerektiğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

