---
title: "IndentatedNode"
second_title: "Справочник API Aspose.Note for Java"
description: "Базовый класс для узлов с относительным отступом для дочерних узлов."
type: docs
weight: 37
url: /ru/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

Базовый класс для узлов с относительным отступом для дочерних узлов.

`T`: Тип элементов в составном узле.

T :
Self :
## Методы

| Метод | Описание |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Получает или задает позицию отступа. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Получает количество элементов, суммируемых в массиве RgOutlineIndentDistance для получения размера отступа. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Получает или задает позицию отступа. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Получает или задает позицию отступа.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Получает количество элементов, суммируемых в массиве RgOutlineIndentDistance для получения размера отступа.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Получает или задает позицию отступа.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

**Returns:**
Self
