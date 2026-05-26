---
title: "Page"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет страницу."
type: docs
weight: 69
url: /ru/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Представляет страницу.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Page()](#Page--) | Инициализирует новый экземпляр класса `Page`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [deepClone()](#deepClone--) | Клонирует страницу. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Клонирует страницу. |
| [getAuthor()](#getAuthor--) | Получает или задаёт автора. |
| [getBackgroundColor()](#getBackgroundColor--) | Получает или задаёт цвет фона страницы. |
| [getCreationTime()](#getCreationTime--) | Получает или задает время создания. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Получает или задает время последнего изменения. |
| [getLevel()](#getLevel--) | Получает или задаёт уровень. |
| [getMargin()](#getMargin--) | Получает или задаёт отступ. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Получает или задаёт сводку ревизии для страницы и её дочерних узлов. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Получает размер макета страницы, отображаемый в редакторе. |
| [getSizeType()](#getSizeType--) | Получает или задаёт тип размера страницы. |
| [getTitle()](#getTitle--) | Получает или задает заголовок. |
| [isConflictPage()](#isConflictPage--) | Получает или задает значение, указывающее, является ли эта страница конфликтной. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Получает или задаёт автора. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Получает или задаёт цвет фона страницы. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Получает или задает значение, указывающее, является ли эта страница конфликтной. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Получает или задает время создания. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Получает или задает время последнего изменения. |
| [setLevel(byte value)](#setLevel-byte-) | Получает или задаёт уровень. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Получает или задаёт отступ. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Получает или задаёт сводку ревизии для страницы и её дочерних узлов. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Устанавливает размер макета страницы, отображаемый в редакторе. |
| [setSizeType(int value)](#setSizeType-int-) | Получает или задаёт тип размера страницы. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Получает или задает заголовок. |
### Page() {#Page--}
```
public Page()
```


Инициализирует новый экземпляр класса `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Клонирует страницу.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Клонирует страницу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cloneHistory | boolean | Указывает, следует ли клонировать историю страницы.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Получает или задаёт автора.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Получает или задаёт цвет фона страницы.

**Returns:**
java.awt.Color
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
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Получает или задаёт уровень.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Получает или задаёт отступ.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Получает или задаёт сводку ревизии для страницы и её дочерних узлов.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Получает размер макета страницы, отображаемый в редакторе.

--------------------

Это значение используется приложением Microsoft OneNote для отображения базового макета страницы при открытии документа. Оно не влияет на печать и сохранение документа. Когда свойство Page.SizeType установлено в PageSizeType.SizeByContent, это свойство возвращает реальный размер содержимого.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Получает или задаёт тип размера страницы.

--------------------

По умолчанию страница автоматически изменяет размер. Значение по умолчанию — [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Получает или задает заголовок.

Значение: `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Получает или задает значение, указывающее, является ли эта страница конфликтной.

--------------------

Конфликтная страница возникает, когда два пользователя пытаются обновить одно и то же содержимое. В этом случае изменения первого пользователя записываются как обычно, но изменения другого пользователя не могут быть объединены. Поэтому создаётся копия страницы и помечается как конфликтная.

В этой версии конфликты разрешаются в пользу изменений первого пользователя. Поэтому, если в документе есть конфликтные страницы, они будут отображаться в истории, но будут пропускаться при сохранении. Можно сбросить этот флаг, чтобы сохранять такие страницы в истории как обычные.

Подробный пример работы с конфликтной страницей можно найти в онлайн‑документации.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Получает или задаёт автора.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Получает или задаёт цвет фона страницы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Получает или задает значение, указывающее, является ли эта страница конфликтной.

--------------------

Конфликтная страница возникает, когда два пользователя пытаются обновить одно и то же содержимое. В этом случае изменения первого пользователя записываются как обычно, но изменения другого пользователя не могут быть объединены. Поэтому создаётся копия страницы и помечается как конфликтная.

В этой версии конфликты разрешаются в пользу изменений первого пользователя. Поэтому, если в документе есть конфликтные страницы, они будут отображаться в истории, но будут пропускаться при сохранении. Можно сбросить этот флаг, чтобы сохранять такие страницы в истории как обычные.

Подробный пример работы с конфликтной страницей можно найти в онлайн‑документации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Получает или задаёт уровень.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Получает или задаёт отступ.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Получает или задаёт сводку ревизии для страницы и её дочерних узлов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Устанавливает размер макета страницы, отображаемый в редакторе.

--------------------

Это значение используется приложением Microsoft OneNote для отображения базового макета страницы при открытии документа. Оно не влияет на печать и сохранение документа. Когда свойство Page.SizeType установлено в PageSizeType.SizeByContent, это свойство возвращает реальный размер содержимого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Получает или задаёт тип размера страницы.

--------------------

По умолчанию страница автоматически изменяет размер. Значение по умолчанию — [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Получает или задает заголовок.

Значение: `Title`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

