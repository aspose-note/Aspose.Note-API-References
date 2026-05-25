---
title: "PageHistory"
second_title: "Aspose.Note for Java API Reference"
description: "Represents the page history."
type: docs
weight: 70
url: /hi/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Represents the page history.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | एक नया उदाहरण `PageHistory` क्लास को आरंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | पेज संस्करण को `PageHistory` के अंत में जोड़ता है। |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | पेज संस्करणों को `PageHistory` के अंत में जोड़ता है। |
| [clear()](#clear--) | पेज इतिहास को साफ़ करता है। |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | निर्धारित करता है कि पेज इतिहास में पेज संस्करण मौजूद है या नहीं। |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Copies the page versions to an array, starting at a particular index.. |
| [getCurrent()](#getCurrent--) | Gets the current page version. |
| [get_Item(int index)](#get-Item-int-) | Gets or sets the page version at the specified index of the `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Determines the index of a specific page version in the page history. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Inserts a page version into the page history. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether the page history is read only. |
| [iterator()](#iterator--) | एक enumerator लौटाता है जो `PageHistory` के चाइल्ड नोड्स के माध्यम से इटररेट करता है। |
| [removeAt(int index)](#removeAt-int-) | निर्दिष्ट इंडेक्स पर `PageHistory` की पेज संस्करण को हटाता है। |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | `PageHistory` से पेज संस्करण को हटाता है। |
| [removeRange(int index, int count)](#removeRange-int-int-) | `PageHistory` से पृष्ठ संस्करणों की एक सीमा हटाता है। |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Gets or sets the page version at the specified index of the `PageHistory`. |
| [size()](#size--) | पृष्ठ इतिहास में पृष्ठ संस्करणों की गिनती प्राप्त करता है। |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


एक नया उदाहरण `PageHistory` क्लास को आरंभ करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | वर्तमान पृष्ठ संस्करण। |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


पेज संस्करण को `PageHistory` के अंत में जोड़ता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | पृष्ठ संस्करण। |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


पेज संस्करणों को `PageHistory` के अंत में जोड़ता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| आइटम्स | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | `IEnumerable\{Page\}` पृष्ठ संस्करणों का संग्रह। |

### clear() {#clear--}
```
public void clear()
```


पेज इतिहास को साफ़ करता है।

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


निर्धारित करता है कि पेज इतिहास में पेज संस्करण मौजूद है या नहीं।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | पृष्ठ संस्करण। |

**Returns:**
boolean - The `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Copies the page versions to an array, starting at a particular index..

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | लक्षित सरणी। |
| arrayIndex | int | सरणी सूचकांक। |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Gets the current page version.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Gets or sets the page version at the specified index of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | सूचकांक। |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Determines the index of a specific page version in the page history.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | पृष्ठ संस्करण। |

**Returns:**
int - The `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Inserts a page version into the page history.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | सूचकांक। |
| item | [Page](../../com.aspose.note/page) | पृष्ठ संस्करण। |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Gets a value indicating whether the page history is read only.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


एक enumerator लौटाता है जो `PageHistory` के चाइल्ड नोड्स के माध्यम से इटररेट करता है।

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`।
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


निर्दिष्ट इंडेक्स पर `PageHistory` की पेज संस्करण को हटाता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | सूचकांक। |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


`PageHistory` से पेज संस्करण को हटाता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | पृष्ठ संस्करण। |

**Returns:**
boolean - The `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


`PageHistory` से पृष्ठ संस्करणों की एक सीमा हटाता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | सूचकांक। |
| count | int | The count. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Gets or sets the page version at the specified index of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | सूचकांक। |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


पृष्ठ इतिहास में पृष्ठ संस्करणों की गिनती प्राप्त करता है।

**Returns:**
int
