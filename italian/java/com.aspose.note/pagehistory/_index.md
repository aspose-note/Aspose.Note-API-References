---
title: "PageHistory"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta la cronologia della pagina."
type: docs
weight: 70
url: /it/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Rappresenta la cronologia della pagina.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Inizializza una nuova istanza della classe `PageHistory`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Aggiunge la versione della pagina alla fine di `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Aggiunge le versioni della pagina alla fine di `PageHistory`. |
| [clear()](#clear--) | Cancella la cronologia delle pagine. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Determina se la cronologia delle pagine contiene la versione della pagina. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Copia le versioni della pagina in un array, a partire da un indice specifico.. |
| [getCurrent()](#getCurrent--) | Ottiene la versione corrente della pagina. |
| [get_Item(int index)](#get-Item-int-) | Ottiene o imposta la versione della pagina all'indice specificato di `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Determina l'indice di una versione specifica della pagina nella cronologia delle pagine. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Inserisce una versione della pagina nella cronologia delle pagine. |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se la cronologia delle pagine è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso i nodi figli di `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Rimuove la versione della pagina all'indice specificato di `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Rimuove la versione della pagina da `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Rimuove un intervallo di versioni della pagina da `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Ottiene o imposta la versione della pagina all'indice specificato di `PageHistory`. |
| [size()](#size--) | Ottiene il conteggio delle versioni della pagina nella cronologia delle pagine. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Inizializza una nuova istanza della classe `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La versione corrente della pagina. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Aggiunge la versione della pagina alla fine di `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versione della pagina. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Aggiunge le versioni della pagina alla fine di `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elementi | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | La collezione `IEnumerable\{Page\}` delle versioni della pagina. |

### clear() {#clear--}
```
public void clear()
```


Cancella la cronologia delle pagine.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Determina se la cronologia delle pagine contiene la versione della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versione della pagina. |

**Returns:**
boolean - Il `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Copia le versioni della pagina in un array, a partire da un indice specifico..

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | L'array di destinazione. |
| arrayIndex | int | L'indice dell'array. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Ottiene la versione corrente della pagina.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Ottiene o imposta la versione della pagina all'indice specificato di `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Determina l'indice di una versione specifica della pagina nella cronologia delle pagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versione della pagina. |

**Returns:**
int - Il `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Inserisce una versione della pagina nella cronologia delle pagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice. |
| item | [Page](../../com.aspose.note/page) | La versione della pagina. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Ottiene un valore che indica se la cronologia delle pagine è di sola lettura.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Restituisce un enumeratore che itera attraverso i nodi figli di `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - L'`IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove la versione della pagina all'indice specificato di `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Rimuove la versione della pagina da `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versione della pagina. |

**Returns:**
boolean - Il `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Rimuove un intervallo di versioni della pagina da `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice. |
| count | int | Il conteggio. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Ottiene o imposta la versione della pagina all'indice specificato di `PageHistory`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Ottiene il conteggio delle versioni della pagina nella cronologia delle pagine.

**Returns:**
int
