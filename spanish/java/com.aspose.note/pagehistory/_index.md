---
title: "PageHistory"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa el historial de la página."
type: docs
weight: 70
url: /es/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Representa el historial de la página.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Inicializa una nueva instancia de la clase `PageHistory`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Agrega la versión de página al final del `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Agrega las versiones de página al final del `PageHistory`. |
| [clear()](#clear--) | Borra el historial de páginas. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Determina si el historial de páginas contiene la versión de página. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Copia las versiones de página a una matriz, comenzando en un índice particular.. |
| [getCurrent()](#getCurrent--) | Obtiene la versión actual de la página. |
| [get_Item(int index)](#get-Item-int-) | Obtiene o establece la versión de página en el índice especificado de `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Determina el índice de una versión de página específica en el historial de páginas. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Inserta una versión de página en el historial de páginas. |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si el historial de páginas es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre los nodos hijos de `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Elimina la versión de página en el índice especificado de `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Elimina la versión de página del `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Elimina un rango de versiones de página del `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Obtiene o establece la versión de página en el índice especificado de `PageHistory`. |
| [size()](#size--) | Obtiene el recuento de versiones de página en el historial de páginas. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Inicializa una nueva instancia de la clase `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | La versión actual de la página. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Agrega la versión de página al final del `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versión de página. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Agrega las versiones de página al final del `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elementos | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | La colección `IEnumerable\\{Page\\}` de versiones de página. |

### clear() {#clear--}
```
public void clear()
```


Borra el historial de páginas.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Determina si el historial de páginas contiene la versión de página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versión de página. |

**Returns:**
boolean - El `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Copia las versiones de página a una matriz, comenzando en un índice particular..

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | La matriz objetivo. |
| arrayIndex | int | El índice de la matriz. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Obtiene la versión actual de la página.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Obtiene o establece la versión de página en el índice especificado de `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | El índice. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Determina el índice de una versión de página específica en el historial de páginas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versión de página. |

**Returns:**
int - El `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Inserta una versión de página en el historial de páginas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | El índice. |
| item | [Page](../../com.aspose.note/page) | La versión de página. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Obtiene un valor que indica si el historial de páginas es de solo lectura.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Devuelve un enumerador que recorre los nodos hijos de `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - El `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina la versión de página en el índice especificado de `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | El índice. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Elimina la versión de página del `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | La versión de página. |

**Returns:**
boolean - El `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Elimina un rango de versiones de página del `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | El índice. |
| count | int | El recuento. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Obtiene o establece la versión de página en el índice especificado de `PageHistory`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | int | El índice. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Obtiene el recuento de versiones de página en el historial de páginas.

**Returns:**
int
