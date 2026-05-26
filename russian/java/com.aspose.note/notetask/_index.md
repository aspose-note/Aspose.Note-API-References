---
title: "NoteTask"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет задачу заметки."
type: docs
weight: 55
url: /ru/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Представляет задачу заметки.
## Методы

| Метод | Описание |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Создаёт новую задачу заметки с иконкой NoFollowUpDateFlag и указанной датой выполнения. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * Создаёт новый тег заметки с иконкой FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * Создаёт новый тег заметки с иконкой FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | * Создаёт новый тег заметки с иконкой FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * Создаёт новый тег заметки с иконкой FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * Создаёт новый тег заметки с иконкой NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Определяет, равен ли указанный объект текущему объекту. |
| [equals(Object obj)](#equals-java.lang.Object-) | Определяет, равен ли указанный объект текущему объекту. |
| [getDueDate()](#getDueDate--) | Получает или задаёт дату выполнения. |
| [getIcon()](#getIcon--) | Получает или задает значок. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Служит хеш-функцией для типа. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Получает или задаёт дату выполнения. |
| [setOpen()](#setOpen--) | Устанавливает тег в открытое состояние. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Создаёт новую задачу заметки с иконкой NoFollowUpDateFlag и указанной датой выполнения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dueDate | java.util.Date | Дата выполнения. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* Создаёт новый тег заметки с иконкой FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* Создаёт новый тег заметки с иконкой FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* Создаёт новый тег заметки с иконкой FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* Создаёт новый тег заметки с иконкой FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* Создаёт новый тег заметки с иконкой NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Определяет, равен ли указанный объект текущему объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | Объект. |

**Returns:**
boolean - Тип `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Определяет, равен ли указанный объект текущему объекту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object | Объект. |

**Returns:**
boolean - Тип `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Получает или задаёт дату выполнения.

Значение: `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Получает или задает значок.

Значение: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Служит хеш-функцией для типа.

**Returns:**
int - Тип `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Получает или задаёт дату выполнения.

Значение: `DateTime`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Устанавливает тег в открытое состояние.

