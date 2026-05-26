---
title: "PageHistory"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar sidans historik."
type: docs
weight: 70
url: /sv/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Representerar sidans historik.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Initierar en ny instans av klassen `PageHistory`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Lägger till sidversionen i slutet av `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Lägger till sidversionerna i slutet av `PageHistory`. |
| [clear()](#clear--) | Rensar sidhistoriken. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Bestämmer om sidhistoriken innehåller sidversionen. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Kopierar sidversionerna till en array, med start vid ett specifikt index.. |
| [getCurrent()](#getCurrent--) | Hämtar den aktuella sidversionen. |
| [get_Item(int index)](#get-Item-int-) | Hämtar eller anger sidversionen vid det angivna indexet i `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Bestämmer indexet för en specifik sidversion i sidhistoriken. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Infogar en sidversion i sidhistoriken. |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om sidhistoriken är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom barnnoderna i `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Tar bort sidversionen vid det angivna indexet i `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Tar bort sidversionen från `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Tar bort ett intervall av sidversionerna från `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Hämtar eller anger sidversionen vid det angivna indexet i `PageHistory`. |
| [size()](#size--) | Hämtar antalet sidversioner i sidhistoriken. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Initierar en ny instans av klassen `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Den aktuella sidversionen. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Lägger till sidversionen i slutet av `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sidversionen. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Lägger till sidversionerna i slutet av `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Den `IEnumerable\\{Page\\}`-samlingen av sidversioner. |

### clear() {#clear--}
```
public void clear()
```


Rensar sidhistoriken.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Bestämmer om sidhistoriken innehåller sidversionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sidversionen. |

**Returns:**
boolean - `bool`-typen.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Kopierar sidversionerna till en array, med start vid ett specifikt index..

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Målarrayen. |
| arrayIndex | int | Arrayindexet. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Hämtar den aktuella sidversionen.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Hämtar eller anger sidversionen vid det angivna indexet i `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Bestämmer indexet för en specifik sidversion i sidhistoriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sidversionen. |

**Returns:**
int - `int`-typen.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Infogar en sidversion i sidhistoriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |
| item | [Page](../../com.aspose.note/page) | Sidversionen. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Hämtar ett värde som indikerar om sidhistoriken är skrivskyddad.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Returnerar en enumerator som itererar genom barnnoderna i `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - Den `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort sidversionen vid det angivna indexet i `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Tar bort sidversionen från `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Sidversionen. |

**Returns:**
boolean - `bool`-typen.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Tar bort ett intervall av sidversionerna från `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |
| count | int | Antalet. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Hämtar eller anger sidversionen vid det angivna indexet i `PageHistory`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Hämtar antalet sidversioner i sidhistoriken.

**Returns:**
int
