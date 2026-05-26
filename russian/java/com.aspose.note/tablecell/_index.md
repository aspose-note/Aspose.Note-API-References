---
title: "TableCell"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет ячейку таблицы."
type: docs
weight: 88
url: /ru/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Представляет ячейку таблицы.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TableCell()](#TableCell--) | Инициализирует новый экземпляр класса `TableCell`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getBackgroundColor()](#getBackgroundColor--) | Возвращает цвет фона. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getMaxWidth()](#getMaxWidth--) | Возвращает максимальную ширину. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Устанавливает цвет фона. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Инициализирует новый экземпляр класса `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Возвращает цвет фона.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Получает количество элементов, суммируемых в массиве RgOutlineIndentDistance для получения размера отступа.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает или задает время последнего изменения.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Возвращает максимальную ширину.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Устанавливает цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Получает или задает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

