---
title: "NotebookSaveOptions"
second_title: "Справочник API Aspose.Note for Java"
description: "Абстрактный базовый класс, представляющий параметры сохранения блокнота для конкретного формата."
type: docs
weight: 61
url: /ru/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Абстрактный базовый класс, представляющий параметры сохранения блокнота для конкретного формата.
## Методы

| Метод | Описание |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Получает или задает значение, указывающее, следует ли сохранять дочерние документы явно. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Получает параметры сохранения для всех дочерних документов блокнота. |
| [getFlatten()](#getFlatten--) | Получает или задает значение, указывающее, сохраняется ли иерархия дочерних элементов блокнота в плоском виде. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат, в котором сохраняется блокнот. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Получает или задает значение, указывающее, следует ли сохранять дочерние документы явно. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Получает или задает значение, указывающее, сохраняется ли иерархия дочерних элементов блокнота в плоском виде. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Получает или задает значение, указывающее, следует ли сохранять дочерние документы явно.

--------------------

Значение по умолчанию — `false`, поэтому дочерние документы будут сохраняться неявно. Значение `true` указывает, что пользователь должен сохранять каждый дочерний узел блокнота явно. Если блокнот сохраняется в поток, значение всегда `true`, несмотря на то, что пользователь явно установил его в `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Получает параметры сохранения для всех дочерних документов блокнота.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Получает или задает значение, указывающее, сохраняется ли иерархия дочерних элементов блокнота в плоском виде.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Получает формат, в котором сохраняется блокнот.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Получает или задает значение, указывающее, следует ли сохранять дочерние документы явно.

--------------------

Значение по умолчанию — `false`, поэтому дочерние документы будут сохраняться неявно. Значение `true` указывает, что пользователь должен сохранять каждый дочерний узел блокнота явно. Если блокнот сохраняется в поток, значение всегда `true`, несмотря на то, что пользователь явно установил его в `false`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Получает или задает значение, указывающее, сохраняется ли иерархия дочерних элементов блокнота в плоском виде.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

