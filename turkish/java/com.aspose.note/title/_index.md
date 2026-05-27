---
title: "Title"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir başlığı temsil eder."
type: docs
weight: 95
url: /tr/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Bir başlığı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Title()](#Title--) | `Title` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Düğüm türüne göre tüm alt düğümleri al. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Yatay ofseti alır veya ayarlar. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getTitleDate()](#getTitleDate--) | Başlıktaki tarihin dize temsili alır veya ayarlar. |
| [getTitleText()](#getTitleText--) | Başlığın metnini alır veya ayarlar. |
| [getTitleTime()](#getTitleTime--) | Başlıktaki zamanın dize temsili alır veya ayarlar. |
| [getVerticalOffset()](#getVerticalOffset--) | Dikey ofseti alır veya ayarlar. |
| [isComposite()](#isComposite--) | Bu düğümün birleşik olup olmadığını gösteren bir değeri alır. |
| [iterator()](#iterator--) | [Title](../../com.aspose.note/title) alt düğümleri arasında yineleme yapan bir enumerator döndürür. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Yatay ofseti alır veya ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Başlıktaki tarihin dize temsili alır veya ayarlar. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Başlığın metnini alır veya ayarlar. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Başlıktaki zamanın dize temsili alır veya ayarlar. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Dikey ofseti alır veya ayarlar. |
### Title() {#Title--}
```
public Title()
```


`Title` sınıfının yeni bir örneğini başlatır.

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
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Yatay ofseti alır veya ayarlar.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Başlıktaki tarihin dize temsili alır veya ayarlar.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Başlığın metnini alır veya ayarlar.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Başlıktaki zamanın dize temsili alır veya ayarlar.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Dikey ofseti alır veya ayarlar.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Bu düğümün birleşik olup olmadığını gösteren bir değeri alır. Doğru ise düğüm alt düğümlere sahip olabilir.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


[Title](../../com.aspose.note/title) alt düğümleri arasında yineleme yapan bir enumerator döndürür.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Yatay ofseti alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Başlıktaki tarihin dize temsili alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Başlığın metnini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Başlıktaki zamanın dize temsili alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Dikey ofseti alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

