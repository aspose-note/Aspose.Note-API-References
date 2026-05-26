---
title: "OutlineElement"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет OutlineElement."
type: docs
weight: 67
url: /ru/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Представляет OutlineElement.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Инициализирует новый экземпляр класса `OutlineElement`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Получает последнего автора элемента контура. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Получает оригинального автора элемента контура. |
| [getCreationTime()](#getCreationTime--) | Получает или задает время создания. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getNumberList()](#getNumberList--) | Получает или задает стиль заголовка нумерованного списка. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Получает или задает время создания. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Получает или задает стиль заголовка нумерованного списка. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Инициализирует новый экземпляр класса `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Получает последнего автора элемента контура.

Значение: Последний автор.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Получает оригинального автора элемента контура.

Значение: Исходный автор.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Получает или задает время создания.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает или задает время последнего изменения.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Получает или задает стиль заголовка нумерованного списка.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Получает или задает время создания.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Получает или задает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Получает или задает стиль заголовка нумерованного списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

