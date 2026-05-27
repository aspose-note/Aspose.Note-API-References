---
title: "GirintiliDüğüm"
second_title: "Aspose.Note for Java API Referansı"
description: "Alt düğümler için göreli girintiye sahip düğümler için temel sınıf."
type: docs
weight: 37
url: /tr/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

Alt düğümler için göreli girintiye sahip düğümler için temel sınıf.

`T`: Bileşik düğümdeki öğelerin türü.

T :
Self :
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Girinti konumunu alır veya ayarlar. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Girinti boyutunu elde etmek için RgOutlineIndentDistance dizisindeki toplanacak öğe sayısını alır. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Girinti konumunu alır veya ayarlar. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Girinti konumunu alır veya ayarlar.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Girinti boyutunu elde etmek için RgOutlineIndentDistance dizisindeki toplanacak öğe sayısını alır.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Girinti konumunu alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

**Returns:**
Self
