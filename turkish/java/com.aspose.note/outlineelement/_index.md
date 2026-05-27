---
title: "OutlineElement"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir OutlineElement'i temsil eder."
type: docs
weight: 67
url: /tr/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Bir OutlineElement'i temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | `OutlineElement` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Bir taslak öğesinin en son yazarını alır. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Bir taslak öğesinin orijinal yazarını alır. |
| [getCreationTime()](#getCreationTime--) | Oluşturma zamanını alır veya ayarlar. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getNumberList()](#getNumberList--) | Numaralı liste başlığı için stili alır veya ayarlar. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Oluşturma zamanını alır veya ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Numaralı liste başlığı için stili alır veya ayarlar. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


`OutlineElement` sınıfının yeni bir örneğini başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Bir taslak öğesinin en son yazarını alır.

Değer: En son yazar.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Bir taslak öğesinin orijinal yazarını alır.

Değer: Orijinal yazar.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Oluşturma zamanını alır veya ayarlar.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Numaralı liste başlığı için stili alır veya ayarlar.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Oluşturma zamanını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Numaralı liste başlığı için stili alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

