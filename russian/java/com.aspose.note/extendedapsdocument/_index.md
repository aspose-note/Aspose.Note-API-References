---
title: "ExtendedApsDocument"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет полный документ one-note, состоящий из Pages, преобразованных в наборы страниц."
type: docs
weight: 23
url: /ru/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

Представляет полный документ OneNote, состоящий из страниц, преобразованных в наборы страниц.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | Инициализирует новый экземпляр класса `ExtendedApsDocument`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | Принимает ApsDocumentVisitor для этого элемента. |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | Добавляет набор страниц в документ. |
| [getPageList()](#getPageList--) | Получает список наборов страниц. |
| [iterator()](#iterator--) | Возвращает перечислитель. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


Инициализирует новый экземпляр класса `ExtendedApsDocument`.

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


Принимает ApsDocumentVisitor для этого элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| посетитель | com.aspose.foundation.rendering.ApsDocumentVisitor | Посетитель. |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


Добавляет набор страниц в документ.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| страница | com.aspose.foundation.rendering.ApsPage | Набор страниц. |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


Получает список наборов страниц.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


Возвращает перечислитель.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
