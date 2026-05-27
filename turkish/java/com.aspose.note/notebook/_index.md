---
title: "Notebook"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir Aspose.Note defterini temsil eder."
type: docs
weight: 56
url: /tr/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Bir Aspose.Note defterini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Notebook()](#Notebook--) | `Notebook` sınıfının yeni bir örneğini başlatır. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | `Notebook` sınıfının yeni bir örneğini başlatır. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | `Notebook` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Düğüm türüne göre tüm alt düğümleri al. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Düğümü listenin sonuna ekler. |
| [getColor()](#getColor--) | Rengi alır veya ayarlar. |
| [getCount()](#getCount--) | `Notebook` içinde bulunan öğe sayısını alır. |
| [getDisplayName()](#getDisplayName--) | Görüntü adını alır veya ayarlar. |
| [getFileFormat()](#getFileFormat--) | Dosya formatını alır (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Nesnenin küresel olarak benzersiz kimliğini alır. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Verilen dizine göre not defteri alt düğümünü alır. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Geçmişin etkin olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [iterator()](#iterator--) | `Notebook` alt düğümleri arasında dolaşan bir yineleyici döndürür. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Bir alt belge düğümü ekler. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Bir alt belge düğümü ekler. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Bir alt belge düğümü ekler. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Bir alt belge düğümü ekler. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Bir alt not defteri düğümü ekler. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Bir alt not defteri düğümü ekler. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Alt düğümü kaldırır. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote belgesini bir akışa kaydeder. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir akışa kaydeder. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | OneNote belgesini belirtilen formatta bir akışa kaydeder. |
| [save(String fileName)](#save-java.lang.String-) | OneNote belgesini bir dosyaya kaydeder. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir dosyaya kaydeder. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | OneNote belgesini belirtilen formatta bir dosyaya kaydeder. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Rengi alır veya ayarlar. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Görüntü adını alır veya ayarlar. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Geçmişin etkin olup olmadığını gösteren bir değeri alır veya ayarlar. |
### Notebook() {#Notebook--}
```
public Notebook()
```


`Notebook` sınıfının yeni bir örneğini başlatır.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


`Notebook` sınıfının yeni bir örneğini başlatır. Bir dosyadan mevcut bir OneNote not defterini açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Yeni bir `Notebook` sınıfı başlatır. Bir dosyadan mevcut bir OneNote defterini açar. "lazy"/instant gibi ek seçenekler, örneğin çocuk yükleme stratejisi, belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Yükleme seçenekleri. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Düğüm türüne göre tüm alt düğümleri al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Çocuk düğümlerin bir listesi.

`T1`: Döndürülen listedeki öğelerin tipi.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Düğümü listenin sonuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Eklenecek düğüm. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Rengi alır veya ayarlar.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


`Notebook` içinde bulunan öğe sayısını alır.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Görüntü adını alır veya ayarlar.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Dosya formatını alır (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Nesnenin küresel olarak benzersiz kimliğini alır.

Değer: GUID.

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


Verilen dizine göre not defteri alt düğümünü alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Çocuk düğümüne indeks. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Geçmişin etkin olup olmadığını gösteren bir değeri alır veya ayarlar.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


`Notebook` alt düğümleri arasında dolaşan bir yineleyici döndürür.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Bir `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Bir çocuk belge düğümü ekler. Bir akıştan mevcut bir OneNote belgesini açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Akış. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Bir çocuk belge düğümü ekler. Bir akıştan mevcut bir OneNote belgesini açar. Ek yükleme seçeneklerini belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Akış. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Yükleme seçenekleri. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Bir çocuk belge düğümü ekler. Bir dosyadan mevcut bir OneNote belgesini açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Bir çocuk belge düğümü ekler. Bir dosyadan mevcut bir OneNote belgesini açar. Ek yükleme seçeneklerini belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Yükleme seçenekleri. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Bir çocuk defter düğümü ekler. Bir dosyadan mevcut bir OneNote defterini açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Bir çocuk defter düğümü ekler. Bir dosyadan mevcut bir OneNote defterini açar. Ek yükleme seçeneklerini belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Yükleme seçenekleri. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Alt düğümü kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Kaldırılacak düğüm. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote belgesini bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Akış. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Akış. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Belgenin nasıl kaydedileceğine dair seçenekleri belirtir. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


OneNote belgesini belirtilen formatta bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Akış. |
| format | int | Belgenin kaydedileceği format. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


OneNote belgesini bir dosyaya kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten mevcutsa, mevcut dosya üzerine yazılır. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir dosyaya kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten mevcutsa, mevcut dosya üzerine yazılır. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Belgenin dosyada nasıl kaydedileceğine ilişkin seçenekleri belirtir. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


OneNote belgesini belirtilen formatta bir dosyaya kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten mevcutsa, mevcut dosya üzerine yazılır. |
| format | int | Belgenin kaydedileceği format. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Rengi alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Görüntü adını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Geçmişin etkin olup olmadığını gösteren bir değeri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

