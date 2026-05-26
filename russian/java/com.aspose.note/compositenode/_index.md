---
title: "CompositeNode"
second_title: "Справочник API Aspose.Note for Java"
description: "Базовый обобщённый класс для узлов, которые могут содержать другие узлы."
type: docs
weight: 15
url: /ru/java/com.aspose.note/compositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT
```
public abstract class CompositeNode<T> extends CompositeNodeBase implements ICompositeNodeT<T>
```

Базовый обобщённый класс для узлов, которые могут содержать другие узлы.

`T`: Тип элементов в составном узле.

T :
## Методы

| Метод | Описание |
| --- | --- |
| [&lt;T1&gt;appendChildFirst(T1 newChild)](#-T1-appendChildFirst-T1-) | Добавляет узел в начало списка дочерних узлов этого узла. |
| [&lt;T1&gt;appendChildLast(T1 newChild)](#-T1-appendChildLast-T1-) | Добавляет узел в конец списка дочерних узлов этого узла. |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Получить все дочерние узлы по типу узла. |
| [&lt;T1&gt;insertChild(int i, T1 newChild)](#-T1-insertChild-int-T1-) | Вставляет узел в указанную позицию списка дочерних узлов этого узла. |
| [&lt;T1&gt;removeChild(T1 oldChild)](#-T1-removeChild-T1-) | Удаляет дочерний узел. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getFirstChild()](#getFirstChild--) | Возвращает первый дочерний узел этого узла. |
| [getLastChild()](#getLastChild--) | Возвращает последний дочерний узел этого узла. |
| [insertChildrenRange(int i, T[] newChildren)](#insertChildrenRange-int-T...-) | Вставляет последовательность узлов, начиная с указанной позиции, в список дочерних узлов этого узла. |
| [insertChildrenRange(int i, Iterable&lt;T&gt; newChildren)](#insertChildrenRange-int-java.lang.Iterable-T--) | Вставляет последовательность узлов, начиная с указанной позиции, в список дочерних узлов этого узла. |
| [isComposite()](#isComposite--) | Проверяет, является ли узел составным. |
| [iterator()](#iterator--) | Возвращает перечислитель, который перебирает дочерние узлы `CompositeNode\{T\}`. |
### &lt;T1&gt;appendChildFirst(T1 newChild) {#-T1-appendChildFirst-T1-}
```
public T1 <T1>appendChildFirst(T1 newChild)
```


Добавляет узел в начало списка дочерних узлов этого узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newChild | T1 | Узел для добавления. |

**Returns:**
T1 - Добавленный узел.
### &lt;T1&gt;appendChildLast(T1 newChild) {#-T1-appendChildLast-T1-}
```
public T1 <T1>appendChildLast(T1 newChild)
```


Добавляет узел в конец списка дочерних узлов этого узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newChild | T1 | Узел для добавления. |

**Returns:**
T1 - Добавленный узел.
### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Получить все дочерние узлы по типу узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Список дочерних узлов.

`T1`: Тип элементов в возвращаемом списке.
### &lt;T1&gt;insertChild(int i, T1 newChild) {#-T1-insertChild-int-T1-}
```
public T1 <T1>insertChild(int i, T1 newChild)
```


Вставляет узел в указанную позицию списка дочерних узлов этого узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| i | int | Позиция для вставки |
| newChild | T1 | Узел для вставки. |

**Returns:**
T1 - Добавленный узел.
### &lt;T1&gt;removeChild(T1 oldChild) {#-T1-removeChild-T1-}
```
public T1 <T1>removeChild(T1 oldChild)
```


Удаляет дочерний узел.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| oldChild | T1 | Узел для удаления. |

**Returns:**
T1 - Удалённый узел.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getFirstChild() {#getFirstChild--}
```
public T getFirstChild()
```


Возвращает первый дочерний узел этого узла.

**Returns:**
T
### getLastChild() {#getLastChild--}
```
public T getLastChild()
```


Возвращает последний дочерний узел этого узла.

**Returns:**
T
### insertChildrenRange(int i, T[] newChildren) {#insertChildrenRange-int-T...-}
```
public final void insertChildrenRange(int i, T[] newChildren)
```


Вставляет последовательность узлов, начиная с указанной позиции, в список дочерних узлов этого узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| i | int | Позиция для вставки |
| newChildren | T[] | Последовательность узлов для вставки. |

### insertChildrenRange(int i, Iterable&lt;T&gt; newChildren) {#insertChildrenRange-int-java.lang.Iterable-T--}
```
public final void insertChildrenRange(int i, Iterable<T> newChildren)
```


Вставляет последовательность узлов, начиная с указанной позиции, в список дочерних узлов этого узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| i | int | Позиция для вставки |
| newChildren | java.lang.Iterable&lt;T&gt; | Последовательность узлов для вставки. |

### isComposite() {#isComposite--}
```
public final boolean isComposite()
```


Проверяет, является ли узел составным. Если true, то узел может иметь дочерние узлы.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<T> iterator()
```


Возвращает перечислитель, который перебирает дочерние узлы `CompositeNode\{T\}`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;T&gt; - `T:IEnumerator`1` для `CompositeNode\{T\}`.
