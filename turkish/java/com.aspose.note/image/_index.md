---
title: "Görsel"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir Görüntüyü temsil eder."
type: docs
weight: 33
url: /tr/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Bir Görüntüyü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | `Image` sınıfının yeni bir örneğini başlatır. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | `Image` sınıfının yeni bir örneğini başlatır. |
| [Image()](#Image--) | `Image` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getAlignment()](#getAlignment--) | Hizalamayı alır. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Görsel için bir gövde alternatif metni alır. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Görsel için alternatif metnin başlığını alır. |
| [getBytes()](#getBytes--) | Görsel veri deposunu alır. |
| [getFileName()](#getFileName--) | Dosya adını alır. |
| [getFilePath()](#getFilePath--) | Görsel dosyasının yolunu alır. |
| [getFormat()](#getFormat--) | Görselin biçimini alır. |
| [getHeight()](#getHeight--) | Yüksekliği alır. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Yatay ofseti alır. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Görsel ile ilişkili köprüyü alır. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanını alır. |
| [getOriginalHeight()](#getOriginalHeight--) | Orijinal yüksekliği alır. |
| [getOriginalWidth()](#getOriginalWidth--) | Orijinal genişliği alır. |
| [getTags()](#getTags--) | Bir görselin tüm etiketlerinin listesini alır. |
| [getVerticalOffset()](#getVerticalOffset--) | Dikey ofseti alır. |
| [getWidth()](#getWidth--) | Genişliği alır. |
| [isBackground()](#isBackground--) | Görselin arka plan görseli olup olmadığını alır. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Mevcut görsel verisini sağlanan Image nesnesinin verisiyle değiştirir. |
| [setAlignment(int value)](#setAlignment-int-) | Hizalamayı ayarlar. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Görsel için bir gövde alternatif metni ayarlar. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Görsel için alternatif metnin başlığını ayarlar. |
| [setBackground(boolean value)](#setBackground-boolean-) | Görselin arka plan görseli olup olmadığını alır. |
| [setHeight(float value)](#setHeight-float-) | Yüksekliği ayarlar. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Yatay ofseti ayarlar. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Görsel ile ilişkili köprüyü ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanını ayarlar. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Dikey ofseti ayarlar. |
| [setWidth(float value)](#setWidth-float-) | Genişliği ayarlar. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


`Image` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | `Image` oluşturulacak dosyanın yolunu içeren bir dizedir. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


`Image` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyaAdı | java.lang.String | Görselin adı. |
| imageStream | java.io.InputStream | Görseli içeren bir akış. |

### Image() {#Image--}
```
public Image()
```


`Image` sınıfının yeni bir örneğini başlatır.

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


Görsel için bir gövde alternatif metni alır.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Görsel için alternatif metnin başlığını alır.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Görsel veri deposunu alır.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Dosya adını alır.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Görsel dosyasının yolunu alır.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Görselin biçimini alır.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Yüksekliği alır. Bu, MS OneNote belgesindeki görselin gerçek yüksekliğidir.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Yatay ofseti alır.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Görsel ile ilişkili köprüyü alır.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanını alır.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Orijinal yüksekliği alır. Bu, yeniden boyutlandırmadan önce görselin orijinal genişliğidir.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Orijinal genişliği alır. Bu, yeniden boyutlandırmadan önce görselin orijinal genişliğidir.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Bir görselin tüm etiketlerinin listesini alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Dikey ofseti alır.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Genişliği alır. Bu, MS OneNote belgesindeki görselin gerçek genişliğidir.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Görselin arka plan görseli olup olmadığını alır.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Mevcut görsel verisini sağlanan Image nesnesinin verisiyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Hizalamayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Görsel için bir gövde alternatif metni ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Görsel için alternatif metnin başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Görselin arka plan görseli olup olmadığını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Yüksekliği ayarlar. Bu, MS OneNote belgesindeki görselin gerçek yüksekliğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Yatay ofseti ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Görsel ile ilişkili köprüyü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Dikey ofseti ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Genişliği ayarlar. Bu, MS OneNote belgesindeki görselin gerçek genişliğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

