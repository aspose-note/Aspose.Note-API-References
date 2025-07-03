---
title: PageHistory
second_title: Aspose.Note for Java API Reference
description: Represents the page history.
type: docs
weight: 70
url: /java/com.aspose.note/pagehistory/
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
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Initializes a new instance of the `PageHistory` class. |
## Methods

| Method | Description |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Adds the page version to the end of the `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Adds the page versions to the end of the `PageHistory`. |
| [clear()](#clear--) | Clears the page history. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Determines whether the page history contains the page version. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Copies the page versions to an array, starting at a particular index.. |
| [getCurrent()](#getCurrent--) | Gets the current page version. |
| [get_Item(int index)](#get-Item-int-) | Gets or sets the page version at the specified index of the `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Determines the index of a specific page version in the page history. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Inserts a page version into the page history. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether the page history is read only. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Removes the page version at the specified index of the `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Removes the page version from the `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Removes a range of the page versions from the `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Gets or sets the page version at the specified index of the `PageHistory`. |
| [size()](#size--) | Gets the count of the page versions in the page history. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Initializes a new instance of the `PageHistory` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | The current page version. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Adds the page version to the end of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | The page version. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Adds the page versions to the end of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| items | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | The `IEnumerable\{Page\}` collection of page versions. |

### clear() {#clear--}
```
public void clear()
```


Clears the page history.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Determines whether the page history contains the page version.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | The page version. |

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
| array | [Page\[\]](../../com.aspose.note/page) | The target array. |
| arrayIndex | int | The array index. |

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
| index | int | The index. |

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
| item | [Page](../../com.aspose.note/page) | The page version. |

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
| index | int | The index. |
| item | [Page](../../com.aspose.note/page) | The page version. |

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


Returns an enumerator that iterates through child nodes of the `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - The `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Removes the page version at the specified index of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Removes the page version from the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | The page version. |

**Returns:**
boolean - The `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Removes a range of the page versions from the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
| count | int | The count. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Gets or sets the page version at the specified index of the `PageHistory`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Gets the count of the page versions in the page history.

**Returns:**
int
