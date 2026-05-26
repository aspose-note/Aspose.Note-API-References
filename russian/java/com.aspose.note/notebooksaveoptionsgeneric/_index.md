---
title: "NotebookSaveOptionsGeneric"
second_title: "Справочник API Aspose.Note for Java"
description: "Абстрактный базовый класс, представляющий параметры сохранения блокнота для конкретного формата и предоставляющий общие параметры сохранения для всех дочерних узлов документа."
type: docs
weight: 62
url: /ru/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

Абстрактный базовый класс, представляющий параметры сохранения блокнота для конкретного формата и предоставляющий общие параметры сохранения для всех дочерних узлов документа.

`TDocumentSaveOptions`: Параметры сохранения для всех дочерних документов блокнота.

TDocumentSaveOptions :
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Получает или задает параметры сохранения для всех дочерних документов блокнота. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Получает параметры сохранения для всех дочерних документов блокнота. |
| [getSaveFormat()](#getSaveFormat--) | Получает формат, в котором сохраняется блокнот. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Получает или задает параметры сохранения для всех дочерних документов блокнота.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Получает параметры сохранения для всех дочерних документов блокнота.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Получает формат, в котором сохраняется блокнот.

**Returns:**
int
