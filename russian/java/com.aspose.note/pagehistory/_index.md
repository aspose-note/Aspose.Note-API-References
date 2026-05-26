---
title: "PageHistory"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет историю страницы."
type: docs
weight: 70
url: /ru/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Представляет историю страницы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Инициализирует новый экземпляр класса `PageHistory`. |
## Методы

| Метод | Описание |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Добавляет версию страницы в конец `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Добавляет версии страниц в конец `PageHistory`. |
| [clear()](#clear--) | Очищает историю страниц. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Определяет, содержит ли история страниц версию страницы. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Копирует версии страниц в массив, начиная с определённого индекса.. |
| [getCurrent()](#getCurrent--) | Получает текущую версию страницы. |
| [get_Item(int index)](#get-Item-int-) | Получает или задаёт версию страницы по указанному индексу `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Определяет индекс конкретной версии страницы в истории страниц. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Вставляет версию страницы в историю страниц. |
| [isReadOnly()](#isReadOnly--) | Получает значение, указывающее, является ли история страниц только для чтения. |
| [iterator()](#iterator--) | Возвращает перечислитель, который перебирает дочерние узлы `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Удаляет версию страницы по указанному индексу `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Удаляет версию страницы из `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Удаляет диапазон версий страниц из `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Получает или задаёт версию страницы по указанному индексу `PageHistory`. |
| [size()](#size--) | Получает количество версий страниц в истории страниц. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Инициализирует новый экземпляр класса `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Текущая версия страницы. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Добавляет версию страницы в конец `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Версия страницы. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Добавляет версии страниц в конец `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| элементы | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Коллекция `IEnumerable\{Page\}` версий страниц. |

### clear() {#clear--}
```
public void clear()
```


Очищает историю страниц.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Определяет, содержит ли история страниц версию страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Версия страницы. |

**Returns:**
boolean - Тип `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Копирует версии страниц в массив, начиная с определённого индекса..

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Целевой массив. |
| arrayIndex | int | Индекс массива. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Получает текущую версию страницы.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Получает или задаёт версию страницы по указанному индексу `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Определяет индекс конкретной версии страницы в истории страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Версия страницы. |

**Returns:**
int - Тип `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Вставляет версию страницы в историю страниц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс. |
| item | [Page](../../com.aspose.note/page) | Версия страницы. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Получает значение, указывающее, является ли история страниц только для чтения.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Возвращает перечислитель, который перебирает дочерние узлы `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удаляет версию страницы по указанному индексу `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Удаляет версию страницы из `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Версия страницы. |

**Returns:**
boolean - Тип `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Удаляет диапазон версий страниц из `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс. |
| count | int | Количество. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Получает или задаёт версию страницы по указанному индексу `PageHistory`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| index | int | Индекс. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Получает количество версий страниц в истории страниц.

**Returns:**
int
