---
title: "AttachedFile"
second_title: "Aspose.Note for Java API Referansı"
description: "Ekli bir dosyayı temsil eder."
type: docs
weight: 11
url: /tr/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Ekli bir dosyayı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | `AttachedFile` sınıfının yeni bir örneğini başlatır. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | `AttachedFile` sınıfının yeni bir örneğini başlatır. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | `AttachedFile` sınıfının yeni bir örneğini başlatır. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | `AttachedFile` sınıfının yeni bir örneğini başlatır. |
| [AttachedFile()](#AttachedFile--) | `AttachedFile` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getAlignment()](#getAlignment--) | Hizalamayı alır. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Ekli dosyanın simgesi için gövde alternatif metnini alır veya ayarlar. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Ekli dosyanın simgesi için alternatif metnin başlığını alır veya ayarlar. |
| [getBytes()](#getBytes--) | Gömülü dosya için ikili veriyi alır. |
| [getExtension()](#getExtension--) | Gömülü dosyanın uzantısını alır. |
| [getFileName()](#getFileName--) | Gömülü dosyanın adını alır. |
| [getFilePath()](#getFilePath--) | Orijinal dosyanın yolunu alır. |
| [getHeight()](#getHeight--) | Gömülü dosya simgesinin orijinal yüksekliğini alır. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Yatay ofseti alır. |
| [getIcon()](#getIcon--) | Gömülü dosyayla ilişkili simge için ikili veriyi alır. |
| [getIconExtension()](#getIconExtension--) | Simgesinin uzantısını alır. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanını alır. |
| [getMaxHeight()](#getMaxHeight--) | Gömülü dosya simgesini görüntülemek için azami yüksekliği alır. |
| [getMaxWidth()](#getMaxWidth--) | Gömülü dosya simgesini görüntülemek için azami genişliği alır. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Dosyaya erişilirken oluşan hata hakkında verileri alır. |
| [getTags()](#getTags--) | Ekli dosyanın etiket listesini alır. |
| [getText()](#getText--) | Gömülü dosyanın metin temsilini alır. |
| [getVerticalOffset()](#getVerticalOffset--) | Dikey ofseti alır. |
| [getWidth()](#getWidth--) | Gömülü dosya simgesinin özgün genişliğini alır. |
| [isPrintout()](#isPrintout--) | Dosyanın görüntüsünün çıktısı olup olmadığını gösteren bir değeri alır. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Simge boyutunun değerinin kullanıcı tarafından açıkça güncellenip güncellenmediğini gösteren bir değeri alır. |
| [setAlignment(int value)](#setAlignment-int-) | Hizalamayı ayarlar. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Ekli dosyanın simgesi için gövde alternatif metnini alır veya ayarlar. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Ekli dosyanın simgesi için alternatif metnin başlığını alır veya ayarlar. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Yatay ofseti ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanını ayarlar. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Gömülü dosya simgesini görüntülemek için azami yüksekliği ayarlar. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Gömülü dosya simgesini görüntülemek için azami genişliği ayarlar. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Dosyanın görüntüsünün çıktısı olup olmadığını gösteren bir değeri ayarlar. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Simge boyutunun değerinin kullanıcı tarafından açıkça güncellenip güncellenmediğini gösteren bir değeri ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Gömülü dosyanın metin temsilini ayarlar. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Dikey ofseti ayarlar. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


`AttachedFile` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | `AttachedFile` oluşturulacak dosyanın yolunu içeren bir dizedir. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


`AttachedFile` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | `AttachedFile` oluşturulacak dosyanın yolunu içeren bir dizedir. |
| simge | java.io.InputStream | Ekli dosya için bir simge. |
| simgeBiçimi | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


`AttachedFile` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Ekli dosyanın adı. |
| attachedFileStream | java.io.InputStream | Ekli dosyanın baytlarını içeren bir akış. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


`AttachedFile` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Ekli dosyanın adı. |
| attachedFileStream | java.io.InputStream | Ekli dosyanın baytlarını içeren bir akış. |
| simge | java.io.InputStream | Ekli dosya için bir simge. |
| simgeBiçimi | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Ekli dosya simgesinin biçimi. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


`AttachedFile` sınıfının yeni bir örneğini başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Hizalamayı alır.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Ekli dosyanın simgesi için gövde alternatif metnini alır veya ayarlar.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Ekli dosyanın simgesi için alternatif metnin başlığını alır veya ayarlar.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Gömülü dosya için ikili veriyi alır.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Gömülü dosyanın uzantısını alır.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Gömülü dosyanın adını alır.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Orijinal dosyanın yolunu alır.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Gömülü dosya simgesinin orijinal yüksekliğini alır.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Yatay ofseti alır.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Gömülü dosyayla ilişkili simge için ikili veriyi alır.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Simgesinin uzantısını alır.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanını alır.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Gömülü dosya simgesini görüntülemek için azami yüksekliği alır.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Gömülü dosya simgesini görüntülemek için azami genişliği alır.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Dosyaya erişilirken oluşan hata hakkında verileri alır.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ekli dosyanın etiket listesini alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Gömülü dosyanın metin temsilini alır. Dize, değer 10 (satır beslemesi) veya 13 (satırbaşı) karakterlerinden herhangi birini içermemelidir.

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Dikey ofseti alır.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Gömülü dosya simgesinin özgün genişliğini alır.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Dosyanın görüntüsünün çıktısı olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Simge boyutunun değerinin kullanıcı tarafından açıkça güncellenip güncellenmediğini gösteren bir değeri alır.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Hizalamayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Alignment'ın değeri. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Ekli dosyanın simgesi için gövde alternatif metnini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Ekli dosyanın simgesi için alternatif metnin başlığını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Yatay ofseti ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | Offsets'ın değeri. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Date'in değeri. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Gömülü dosya simgesini görüntülemek için azami yüksekliği ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | Maksimum yüksekliğin değeri. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Gömülü dosya simgesini görüntülemek için azami genişliği ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | Maksimum genişliğin değeri. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Dosyanın görüntüsünün çıktısı olup olmadığını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Yeni değer. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Simge boyutunun değerinin kullanıcı tarafından açıkça güncellenip güncellenmediğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Yeni değer. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Gömülü dosyanın metin temsilini ayarlar. Dize, değer 10 (satır beslemesi) veya 13 (satırbaşı) karakterlerinden herhangi birini içermemelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Text'in değeri. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Dikey ofseti ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | Offset'in değeri. |

