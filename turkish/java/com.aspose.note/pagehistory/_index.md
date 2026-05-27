---
title: "PageHistory"
second_title: "Aspose.Note for Java API Referansı"
description: "Sayfa geçmişini temsil eder."
type: docs
weight: 70
url: /tr/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Sayfa geçmişini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Yeni bir `PageHistory` sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Sayfa sürümünü `PageHistory`'nin sonuna ekler. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Sayfa sürümlerini `PageHistory`'nin sonuna ekler. |
| [clear()](#clear--) | Sayfa geçmişini temizler. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Sayfa geçmişinin sayfa sürümünü içerip içermediğini belirler. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Sayfa sürümlerini bir diziye kopyalar, belirli bir indeksten başlayarak.. |
| [getCurrent()](#getCurrent--) | Geçerli sayfa sürümünü alır. |
| [get_Item(int index)](#get-Item-int-) | `PageHistory`'nin belirtilen indeksindeki sayfa sürümünü alır veya ayarlar. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Sayfa geçmişindeki belirli bir sayfa sürümünün indeksini belirler. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Sayfa sürümünü sayfa geçmişine ekler. |
| [isReadOnly()](#isReadOnly--) | Sayfa geçmişinin yalnızca okunur olup olmadığını gösteren bir değeri alır. |
| [iterator()](#iterator--) | `PageHistory`'nin alt düğümleri arasında yineleme yapan bir enumeratörü döndürür. |
| [removeAt(int index)](#removeAt-int-) | `PageHistory`'nin belirtilen indeksindeki sayfa sürümünü kaldırır. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Sayfa sürümünü `PageHistory`'den kaldırır. |
| [removeRange(int index, int count)](#removeRange-int-int-) | `PageHistory`'den sayfa sürümlerinin bir aralığını kaldırır. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | `PageHistory`'nin belirtilen indeksindeki sayfa sürümünü alır veya ayarlar. |
| [size()](#size--) | Sayfa geçmişindeki sayfa sürümlerinin sayısını alır. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Yeni bir `PageHistory` sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Geçerli sayfa sürümü. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Sayfa sürümünü `PageHistory`'nin sonuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sayfa sürümü. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Sayfa sürümlerini `PageHistory`'nin sonuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğeler | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Sayfa sürümlerinin `IEnumerable\{Page\}` koleksiyonu. |

### clear() {#clear--}
```
public void clear()
```


Sayfa geçmişini temizler.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Sayfa geçmişinin sayfa sürümünü içerip içermediğini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sayfa sürümü. |

**Returns:**
boolean - Bu `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Sayfa sürümlerini bir diziye kopyalar, belirli bir indeksten başlayarak..

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Hedef dizi. |
| arrayIndex | int | Dizi indeksi. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Geçerli sayfa sürümünü alır.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


`PageHistory`'nin belirtilen indeksindeki sayfa sürümünü alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | İndeks. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Sayfa geçmişindeki belirli bir sayfa sürümünün indeksini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sayfa sürümü. |

**Returns:**
int - Bu `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Sayfa sürümünü sayfa geçmişine ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | İndeks. |
| item | [Page](../../com.aspose.note/page) | Sayfa sürümü. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Sayfa geçmişinin yalnızca okunur olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


`PageHistory`'nin alt düğümleri arasında yineleme yapan bir enumeratörü döndürür.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


`PageHistory`'nin belirtilen indeksindeki sayfa sürümünü kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | İndeks. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Sayfa sürümünü `PageHistory`'den kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sayfa sürümü. |

**Returns:**
boolean - Bu `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


`PageHistory`'den sayfa sürümlerinin bir aralığını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | İndeks. |
| count | int | Sayım. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


`PageHistory`'nin belirtilen indeksindeki sayfa sürümünü alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | İndeks. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Sayfa geçmişindeki sayfa sürümlerinin sayısını alır.

**Returns:**
int
