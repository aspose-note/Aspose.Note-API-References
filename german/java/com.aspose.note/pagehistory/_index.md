---
title: "PageHistory"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt die Seitenhistorie dar."
type: docs
weight: 70
url: /de/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Stellt die Seitenhistorie dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Initialisiert eine neue Instanz der Klasse `PageHistory`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Fügt die Seitenversion am Ende von `PageHistory` hinzu. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Fügt die Seitenversionen am Ende von `PageHistory` hinzu. |
| [clear()](#clear--) | Löscht die Seitenhistorie. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Bestimmt, ob die Seitenhistorie die Seitenversion enthält. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Kopiert die Seitenversionen in ein Array, beginnend bei einem bestimmten Index.. |
| [getCurrent()](#getCurrent--) | Gibt die aktuelle Seitenversion zurück. |
| [get_Item(int index)](#get-Item-int-) | Liest oder setzt die Seitenversion am angegebenen Index des `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Bestimmt den Index einer bestimmten Seitenversion in der Seitenhistorie. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Fügt eine Seitenversion in die Seitenhistorie ein. |
| [isReadOnly()](#isReadOnly--) | Liefert einen Wert, der angibt, ob die Seitenhistorie schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die Kindknoten des `PageHistory` durchläuft. |
| [removeAt(int index)](#removeAt-int-) | Entfernt die Seitenversion am angegebenen Index des `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Entfernt die Seitenversion aus dem `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Entfernt einen Bereich von Seitenversionen aus dem `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Liest oder setzt die Seitenversion am angegebenen Index des `PageHistory`. |
| [size()](#size--) | Liefert die Anzahl der Seitenversionen in der Seitenhistorie. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Initialisiert eine neue Instanz der Klasse `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Die aktuelle Seitenversion. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Fügt die Seitenversion am Ende von `PageHistory` hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Die Seitenversion. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Fügt die Seitenversionen am Ende von `PageHistory` hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Elemente | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Die `IEnumerable\{Page\}`-Sammlung von Seitenversionen. |

### clear() {#clear--}
```
public void clear()
```


Löscht die Seitenhistorie.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Bestimmt, ob die Seitenhistorie die Seitenversion enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Die Seitenversion. |

**Returns:**
boolean - Der `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Kopiert die Seitenversionen in ein Array, beginnend bei einem bestimmten Index..

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Das Zielarray. |
| arrayIndex | int | Der Array-Index. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Gibt die aktuelle Seitenversion zurück.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Liest oder setzt die Seitenversion am angegebenen Index des `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Der Index. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Bestimmt den Index einer bestimmten Seitenversion in der Seitenhistorie.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Die Seitenversion. |

**Returns:**
int - Der `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Fügt eine Seitenversion in die Seitenhistorie ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Der Index. |
| item | [Page](../../com.aspose.note/page) | Die Seitenversion. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Liefert einen Wert, der angibt, ob die Seitenhistorie schreibgeschützt ist.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Gibt einen Enumerator zurück, der die Kindknoten des `PageHistory` durchläuft.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - Der `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt die Seitenversion am angegebenen Index des `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Der Index. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Entfernt die Seitenversion aus dem `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Die Seitenversion. |

**Returns:**
boolean - Der `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Entfernt einen Bereich von Seitenversionen aus dem `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Der Index. |
| count | int | Die Anzahl. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Liest oder setzt die Seitenversion am angegebenen Index des `PageHistory`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | Der Index. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Liefert die Anzahl der Seitenversionen in der Seitenhistorie.

**Returns:**
int
