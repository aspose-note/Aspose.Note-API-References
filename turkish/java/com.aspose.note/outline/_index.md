---
title: "Ana Hat"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir taslağı temsil eder."
type: docs
weight: 66
url: /tr/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Bir taslağı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Outline()](#Outline--) | Yeni bir [Outline](../../com.aspose.note/outline) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Outline'ın alt öğelerinin taşınıp taşınabileceğini alır. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Yatay ofseti alır veya ayarlar. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getMaxHeight()](#getMaxHeight--) | Azami yüksekliği alır veya ayarlar. |
| [getMaxWidth()](#getMaxWidth--) | Azami genişliği alır veya ayarlar. |
| [getMinWidth()](#getMinWidth--) | Minimum genişliği alır veya ayarlar. |
| [getReservedWidth()](#getReservedWidth--) | Ayrılmış genişliği alır veya ayarlar. |
| [getVerticalOffset()](#getVerticalOffset--) | Dikey ofseti alır veya ayarlar. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Outline'ın alt öğelerinin taşınıp taşınabileceğini alır. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Yatay ofseti alır veya ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Azami yüksekliği alır veya ayarlar. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Azami genişliği alır veya ayarlar. |
| [setMinWidth(float value)](#setMinWidth-float-) | Minimum genişliği alır veya ayarlar. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Ayrılmış genişliği alır veya ayarlar. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Dikey ofseti alır veya ayarlar. |
### Outline() {#Outline--}
```
public Outline()
```


Yeni bir [Outline](../../com.aspose.note/outline) sınıfı örneği başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` sınıfından türetilen bir sınıfın nesnesi. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Outline'ın alt öğelerinin taşınıp taşınabileceğini alır.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Yatay ofseti alır veya ayarlar.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Girinti boyutunu elde etmek için RgOutlineIndentDistance dizisindeki toplanacak öğe sayısını alır.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Azami yüksekliği alır veya ayarlar.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Azami genişliği alır veya ayarlar.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Minimum genişliği alır veya ayarlar.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Ayrılmış genişliği alır veya ayarlar.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Dikey ofseti alır veya ayarlar.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Outline'ın alt öğelerinin taşınıp taşınabileceğini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
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

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Azami yüksekliği alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Azami genişliği alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Minimum genişliği alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Ayrılmış genişliği alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Dikey ofseti alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

