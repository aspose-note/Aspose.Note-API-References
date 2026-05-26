---
title: "PageHistory"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt de paginageschiedenis voor."
type: docs
weight: 70
url: /nl/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Stelt de paginageschiedenis voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Initialiseert een nieuw exemplaar van de `PageHistory`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Voegt de paginaversie toe aan het einde van de `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Voegt de paginaversies toe aan het einde van de `PageHistory`. |
| [clear()](#clear--) | Leegt de paginageschiedenis. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Bepaalt of de paginageschiedenis de paginaversie bevat. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Kopieert de paginaversies naar een array, beginnend bij een bepaalde index.. |
| [getCurrent()](#getCurrent--) | Haalt de huidige paginaversie op. |
| [get_Item(int index)](#get-Item-int-) | Haalt op of stelt de paginaversie in op de opgegeven index van de `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Bepaalt de index van een specifieke paginaversie in de paginageschiedenis. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Voegt een paginaversie in de paginageschiedenis in. |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of de paginageschiedenis alleen-lezen is. |
| [iterator()](#iterator--) | Retourneert een enumerator die door de kindknopen van de `PageHistory` iterereert. |
| [removeAt(int index)](#removeAt-int-) | Verwijdert de paginaversie op de opgegeven index van de `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Verwijdert de paginaversie uit de `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Verwijdert een reeks paginaversies uit de `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Haalt op of stelt de paginaversie in op de opgegeven index van de `PageHistory`. |
| [size()](#size--) | Haalt het aantal paginaversies op in de paginageschiedenis. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Initialiseert een nieuw exemplaar van de `PageHistory`-klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | De huidige paginaversie. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Voegt de paginaversie toe aan het einde van de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | De paginaversie. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Voegt de paginaversies toe aan het einde van de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| items | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | De `IEnumerable\{Page\}` collectie van paginaversies. |

### clear() {#clear--}
```
public void clear()
```


Leegt de paginageschiedenis.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Bepaalt of de paginageschiedenis de paginaversie bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | De paginaversie. |

**Returns:**
boolean - De `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Kopieert de paginaversies naar een array, beginnend bij een bepaalde index..

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | De doelarray. |
| arrayIndex | int | De array-index. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Haalt de huidige paginaversie op.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Haalt op of stelt de paginaversie in op de opgegeven index van de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De index. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Bepaalt de index van een specifieke paginaversie in de paginageschiedenis.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | De paginaversie. |

**Returns:**
int - De `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Voegt een paginaversie in de paginageschiedenis in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De index. |
| item | [Page](../../com.aspose.note/page) | De paginaversie. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Haalt een waarde op die aangeeft of de paginageschiedenis alleen-lezen is.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Retourneert een enumerator die door de kindknopen van de `PageHistory` iterereert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - De `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Verwijdert de paginaversie op de opgegeven index van de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De index. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Verwijdert de paginaversie uit de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | De paginaversie. |

**Returns:**
boolean - De `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Verwijdert een reeks paginaversies uit de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De index. |
| count | int | Het aantal. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Haalt op of stelt de paginaversie in op de opgegeven index van de `PageHistory`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De index. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Haalt het aantal paginaversies op in de paginageschiedenis.

**Returns:**
int
