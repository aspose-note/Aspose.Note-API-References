---
title: "Document"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir Aspose.Note belgesini temsil eder."
type: docs
weight: 20
url: /tr/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Bir Aspose.Note belgesini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Document()](#Document--) | `Document` sınıfının yeni bir örneğini başlatır. |
| [Document(String filePath)](#Document-java.lang.String-) | `Document` sınıfının yeni bir örneğini başlatır. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | `Document` sınıfının yeni bir örneğini başlatır. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | `Document` sınıfının yeni bir örneğini başlatır. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | `Document` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [detectLayoutChanges()](#detectLayoutChanges--) | `DetectLayoutChanges` çağrısından bu yana belge düzeninde yapılan tüm değişiklikleri algılar. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Aspose.Note'un düzen değişikliklerini otomatik olarak algılayıp algılamadığını gösteren değeri alır. |
| [getColor()](#getColor--) | Rengi alır. |
| [getCreationTime()](#getCreationTime--) | Oluşturulma zamanını alır. |
| [getDisplayName()](#getDisplayName--) | Görüntülenen adı alır. |
| [getFileFormat()](#getFileFormat--) | Dosya formatını alır (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Nesnenin küresel olarak benzersiz kimliğini alır. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Belgedeki her sayfa için tam geçmişi içeren `PageHistory` öğesini alır (en eski 0. indeksde). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. |
| [print()](#print--) | Belgeyi varsayılan yazıcıyla yazdırır. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Belgeyi varsayılan yazıcıyla yazdırır. |
| [print(String printerName)](#print-java.lang.String-) | Belgeyi varsayılan yazıcıyla yazdırır. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Belgeyi varsayılan yazıcıyla yazdırır. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote belgesini bir akışa kaydeder. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir akışa kaydeder. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | OneNote belgesini belirtilen formatta bir akışa kaydeder. |
| [save(String fileName)](#save-java.lang.String-) | OneNote belgesini bir dosyaya kaydeder. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir dosyaya kaydeder. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | OneNote belgesini belirtilen formatta bir dosyaya kaydeder. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Aspose.Note'un yerleşim değişikliklerini otomatik olarak algılayıp algılamadığını gösteren bir değer ayarlar. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Rengi ayarlar. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Oluşturma zamanını ayarlar. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Görünen adı ayarlar. |
### Document() {#Document--}
```
public Document()
```


`Document` sınıfının yeni bir örneğini başlatır. Boş bir OneNote belgesi oluşturur.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


`Document` sınıfının yeni bir örneğini başlatır. Bir dosyadan mevcut bir OneNote belgesi açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


`Document` sınıfının yeni bir örneğini başlatır. Bir dosyadan mevcut bir OneNote belgesi açar. Şifreleme parolası gibi ek seçenekler belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Bir belgeyi yüklemek için kullanılan seçenekler. Null olabilir. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


`Document` sınıfının yeni bir örneğini başlatır. Bir akıştan mevcut bir OneNote belgesi açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inStream | java.io.InputStream | Akış. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


`Document` sınıfının yeni bir örneğini başlatır. Bir akıştan mevcut bir OneNote belgesi açar. Şifreleme parolası gibi ek seçenekler belirtmeye izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inStream | java.io.InputStream | Akış. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Bir belgeyi yüklemek için kullanılan seçenekler. Null olabilir. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Belge yerleşiminde önceki `DetectLayoutChanges` çağrısından bu yana yapılan tüm değişiklikleri algılar. `AutomaticLayoutChangesDetectionEnabled` true olarak ayarlanmışsa, belge dışa aktarımının başında otomatik olarak kullanılır.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Aspose.Note'un yerleşim değişikliklerini otomatik olarak algılayıp algılamadığını gösteren bir değeri alır. Varsayılan değer `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Rengi alır.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Oluşturulma zamanını alır.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Görüntülenen adı alır.

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


`PageHistory` öğesini alır; bu öğe bir belgede sunulan her sayfanın tam geçmişini içerir (en eski 0. indekstedir). Mevcut sayfa revizyonuna `PageHistory.current` olarak erişilebilir ve tarihsel sürüm koleksiyonundan ayrı tutulur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Bir sayfanın mevcut revizyonu. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Akış. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Akış. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Yükleme seçenekleri. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Bir akıştan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Akış. |
| password | java.lang.String | Bir belgeyi çözmek için kullanılan şifre. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Yükleme seçenekleri. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Bir dosyadan gelen belgenin şifrelenip şifrelenmediğini kontrol eder. Kontrol etmek için belgeyi tamamen yüklememiz gerekir. Bu nedenle bu yöntem performans cezasına yol açabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu. |
| password | java.lang.String | Bir belgeyi çözmek için kullanılan şifre. |
| document | [Document\[\]](../../com.aspose.note/document) | Yüklenen belge. |

**Returns:**
boolean - Belge şifreli ise true, aksi takdirde false döndürür.
### print() {#print--}
```
public void print()
```


Belgeyi varsayılan yazıcıyla yazdırır.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Belgeyi varsayılan yazıcıyla yazdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Bir belgeyi yazdırmak için kullanılan seçenekler. Null olabilir. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Belgeyi varsayılan yazıcıyla yazdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Belgeyi varsayılan yazıcıyla yazdırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote belgesini bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Belgenin kaydedileceği System.iO.stream. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Belgenin kaydedileceği System.iO.stream. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Belgenin akışta nasıl kaydedileceğine ilişkin seçenekleri belirtir. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


OneNote belgesini belirtilen formatta bir akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.OutputStream | Belgenin kaydedileceği System.iO.stream. |
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

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


OneNote belgesini belirtilen kaydetme seçeneklerini kullanarak bir dosyaya kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Dosyanın tam adı. Belirtilen tam ada sahip bir dosya zaten mevcutsa, mevcut dosya üzerine yazılır. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Belgenin dosyada nasıl kaydedileceğine ilişkin seçenekleri belirtir. |

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

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Aspose.Note'un yerleşim değişikliklerini otomatik olarak algılayıp algılamadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Yeni değer. Null olabilir. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Rengi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | Renk değeri. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Oluşturma zamanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | DateTime değeri. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Görünen adı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | DateTime değeri. |

