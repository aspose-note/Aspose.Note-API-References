---
title: "Title"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет заголовок."
type: docs
weight: 95
url: /ru/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Представляет заголовок.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Title()](#Title--) | Инициализирует новый экземпляр класса `Title`. |
## Методы

| Метод | Описание |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Получить все дочерние узлы по типу узла. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Получает или задает горизонтальное смещение. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getTitleDate()](#getTitleDate--) | Получает или задает строковое представление даты в заголовке. |
| [getTitleText()](#getTitleText--) | Получает или задает текст заголовка. |
| [getTitleTime()](#getTitleTime--) | Получает или задает строковое представление времени в заголовке. |
| [getVerticalOffset()](#getVerticalOffset--) | Получает или задает вертикальное смещение. |
| [isComposite()](#isComposite--) | Получает значение, указывающее, является ли этот узел составным. |
| [iterator()](#iterator--) | Возвращает перечислитель, который перебирает дочерние узлы [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Получает или задает горизонтальное смещение. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Получает или задает строковое представление даты в заголовке. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Получает или задает текст заголовка. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Получает или задает строковое представление времени в заголовке. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Получает или задает вертикальное смещение. |
### Title() {#Title--}
```
public Title()
```


Инициализирует новый экземпляр класса `Title`.

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
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| тип | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Получает или задает горизонтальное смещение.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Получает или задает время последнего изменения.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Получает или задает строковое представление даты в заголовке.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Получает или задает текст заголовка.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Получает или задает строковое представление времени в заголовке.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Получает или задает вертикальное смещение.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Возвращает перечислитель, который перебирает дочерние узлы [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - Перечислитель.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
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

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Получает или задает строковое представление даты в заголовке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Получает или задает текст заголовка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Получает или задает строковое представление времени в заголовке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Получает или задает вертикальное смещение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | float |  |

