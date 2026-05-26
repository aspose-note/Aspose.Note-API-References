---
title: "ExtendedApsPage"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет обёртку для стандартных ApsGlyphs, которая расширяет часть поведения отрисовки."
type: docs
weight: 27
url: /ru/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Представляет обёртку для стандартных ApsGlyphs, которая расширяет часть поведения рисования.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Инициализирует новый экземпляр класса `ExtendedApsPage`. |
## Методы

| Метод | Описание |
| --- | --- |
| [getContentSize()](#getContentSize--) | Получает размер страницы без учёта полей. |
| [getMargin()](#getMargin--) | Получает поля этой страницы. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Получает позицию конца страницы в MS OneNote, когда одна страница MS OneNote разделена на несколько страниц aps. |
| [getPageSize()](#getPageSize--) | Получает окончательный размер страницы. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Получает позицию начала страницы в MS OneNote, когда одна страница MS OneNote разделена на несколько страниц aps. |
| [iterator()](#iterator--) | Возвращает перечислитель, который перебирает все узлы этой страницы. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Получить перечислитель. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Инициализирует новый экземпляр класса `ExtendedApsPage`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Размер страницы. |
| pageStartInNotePage | float | Начало страницы в оригинальной странице MS OneNote. |
| margin | com.aspose.foundation.layout.Margin | Расширенный отступ страницы. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Получает размер страницы без учёта полей.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Получает поля этой страницы.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Получает позицию конца страницы в MS OneNote, когда одна страница MS OneNote разделена на несколько страниц aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Получает окончательный размер страницы.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Получает позицию начала страницы в MS OneNote, когда одна страница MS OneNote разделена на несколько страниц aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Возвращает перечислитель, который перебирает все узлы этой страницы.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Интерфейс `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Получить перечислитель.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Интерфейс `IEnumerator`.
