---
title: "ITag"
second_title: "Справочник API Aspose.Note for Java"
description: "Интерфейс для тегов всех видов."
type: docs
weight: 109
url: /ru/java/com.aspose.note/itag/
---
```
public interface ITag
```

Интерфейс для тегов всех видов.
## Методы

| Метод | Описание |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Получает время завершения. |
| [getCreationTime()](#getCreationTime--) | Получает время создания. |
| [getIcon()](#getIcon--) | Получает значок. |
| [getLabel()](#getLabel--) | Получает текст метки. |
| [getStatus()](#getStatus--) | Получает статус. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Устанавливает время создания. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Получает время завершения.

Значение: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Получает время создания.

Значение: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Получает значок.

Значение: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Получает текст метки.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Получает статус.

Значение: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Устанавливает время создания.

Значение: java.util.Date.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

