---
title: "Outline"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет структуру."
type: docs
weight: 66
url: /ru/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Представляет структуру.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Outline()](#Outline--) | Инициализирует новый экземпляр класса [Outline](../../com.aspose.note/outline). |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Получает, могут ли потомки контура перемещаться. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Получает или задает горизонтальное смещение. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getMaxHeight()](#getMaxHeight--) | Получает или задает максимальную высоту. |
| [getMaxWidth()](#getMaxWidth--) | Получает или задает максимальную ширину. |
| [getMinWidth()](#getMinWidth--) | Получает или задает минимальную ширину. |
| [getReservedWidth()](#getReservedWidth--) | Получает или задает зарезервированную ширину. |
| [getVerticalOffset()](#getVerticalOffset--) | Получает или задает вертикальное смещение. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Получает, могут ли потомки контура перемещаться. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Получает или задает горизонтальное смещение. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Получает или задает максимальную высоту. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Получает или задает максимальную ширину. |
| [setMinWidth(float value)](#setMinWidth-float-) | Получает или задает минимальную ширину. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Получает или задает зарезервированную ширину. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Получает или задает вертикальное смещение. |
### Outline() {#Outline--}
```
public Outline()
```


Инициализирует новый экземпляр класса [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Получает, могут ли потомки контура перемещаться.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Получает или задает горизонтальное смещение.

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Получает или задает максимальную высоту.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Получает или задает максимальную ширину.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Получает или задает минимальную ширину.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Получает или задает зарезервированную ширину.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Получает или задает вертикальное смещение.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Получает, могут ли потомки контура перемещаться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Получает или задает горизонтальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Получает или задает время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Получает или задает максимальную высоту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Получает или задает максимальную ширину.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Получает или задает минимальную ширину.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Получает или задает зарезервированную ширину.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Получает или задает вертикальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

